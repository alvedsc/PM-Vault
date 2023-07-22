---
{"dg-publish":true,"permalink":"/cards/classification/"}
---

up:: [[Supervised Learning\|Supervised Learning]] 
d:: c

Instad of predicting a numeric value, like in the case of [[Linear Regression\|Linear Regression]], we want to predict a category. 

An example of classification is [[Image Classification\|Image Classification]] 

The output we expect is the probability that an input belongs to each of the output classes 

We will run the example in this [Jupyter Notebook](https://colab.research.google.com/drive/15Cyy2H7nT40sGR7TBN5wBvgTd57mVKay#forceEdit=true&sandboxMode=true&scrollTo=JQz0Lj60hjLI) 

```python
# First we initialize the code
%tensorflow_version 2.x # this line is not required unless you are in a notebook

from __future__ import absolute_import, division, print_function, unicode_literals
import tensorflow as tf
import pandas as pd
```

We will use the iris flower dataset. 

This specific dataset seperates flowers into 3 different classes of species.
{ #b66c11}

-   Setosa
-   Versicolor
-   Virginica

The information about each flower is the following.
-   sepal length
-   sepal width
-   petal length
-   petal width

The idea is to train a model to classify flowers by their input parameters

Now let's define vector constants for later use:
```python
CSV_COLUMN_NAMES = ['SepalLength', 'SepalWidth', 'PetalLength', 'PetalWidth', 'Species']
SPECIES = ['Setosa', 'Versicolor', 'Virginica']
# Lets define some constants to help us later on
```

Extract the data set into a variable 
```python
train_path = tf.keras.utils.get_file(
"iris_training.csv", "https://storage.googleapis.com/download.tensorflow.org/data/iris_training.csv")

test_path = tf.keras.utils.get_file(
"iris_test.csv", "https://storage.googleapis.com/download.tensorflow.org/data/iris_test.csv")

train = pd.read_csv(train_path, names=CSV_COLUMN_NAMES, header=0)
test = pd.read_csv(test_path, names=CSV_COLUMN_NAMES, header=0)
# Here we use keras (a module inside of TensorFlow) to grab our datasets and read them into a pandas dataframe
```

`train.head()` will output: 
![[Classification.09-02-2023-1.png\|Classification.09-02-2023-1.png]]

As you can see, the species classes are already encoded, so it will not be necessary to do the dictionary part we did in [[Linear Regression#^062788\|Linear Regression#^062788]] 

Extract the labels, using `.pop`
```python
train_y = train.pop('Species')
test_y = test.pop('Species')
```

Now define the [[Input Function\|Input Function]] 
```python
def input_fn(features, labels, training=True, batch_size=256):
	
	# Convert the inputs to a Dataset.
	dataset = tf.data.Dataset.from_tensor_slices((dict(features), labels))
	
	# Shuffle and repeat if you are in training mode.
	if training:
		dataset = dataset.shuffle(1000).repeat()
	return dataset.batch(batch_size)
```

Notice this [[Input Function\|Input Function]] is considerably simpler than the one in the [[Linear Regression#^449764\|Linear Regression#^449764]]. Main difference is the absense of epochs, so the pass is only repeated once, after shuffling 

Then we need to create the feature columns in the format we discussed in [[Linear Regression\|Linear Regression]] so the model knows how to use the inputs. However, in this case there are no categorical columns so there will only be one `for loop` 

```python
# Feature columns describe how to use the input.
my_feature_columns = []
for key in train.keys():
	my_feature_columns.append(tf.feature_column.numeric_column(key=key))
```

### Building the model
There are many classification premade models in [[TensorFlow\|TensorFlow]]. However, the best for this case will be the Deep Neural Network model 

```python
# Build a DNN with 2 hidden layers with 30 and 10 hidden nodes each.
classifier = tf.estimator.DNNClassifier(
	feature_columns=my_feature_columns,
	# Two hidden layers of 30 and 10 nodes respectively.
	hidden_units=[30, 10],
	# The model must choose between 3 classes.
n_classes=3)
```

Let's digest this:
- The `.estimator` module is a storage for many models, including DNNClassifier 
- `hidden_units` determines the dimension of the hidden layers. In this case, the model will use two hidden layers with 30 and 10 nodes respectively 
- The model chooses between 3 classes as determined in [[Cards/Classification#^b66c11\|#^b66c11]]

### Train the model
```python
classifier.train(
	input_fn=lambda: input_fn(train, train_y, training=True),
	steps=5000)
# We include a lambda to avoid creating an inner function previously
```

Let's digest this:
- a `Lambda` is a property of Python that allows you to define a function in one line (just like we see above) 
	- Since the function `input_fn` outputs a `dataset`, then the line `lambda: input_fn(train, train_y, training=True)` will define a function as the output of the `input_fn` 
		- In the case of the [[Linear Regression#^449764\|Linear Regression#^449764]] we did not have to do this, since the function make_input_function(...) returns the inner function. 
		- Either of the two ways is correct
- In this case, we did not run the model through a number of epochs. 
	- Instead, we input a `steps = 5000` so that the model runs until it looks at 5000 pieces of data, regardless of the number of epochs that implies 
- Note: we train the model in [[Keras\|Keras]] differently. In keras we use the `.model.fit()` function. 

### Evaluate the model 
```python
eval_result = classifier.evaluate(
	input_fn=lambda: input_fn(test, test_y, training=False))
print('\nTest set accuracy: {accuracy:0.3f}\n'.format(**eval_result))
# The last line is so that the accuracy result comes in a better format 
```

### Prediction
You can run a prediction jsut like you did in [[Linear Regression#^ac1d01\|Linear Regression#^ac1d01]] 

However, here's a function to generate a prediction on an input feature 
```python
def input_fn(features, batch_size=256):
    # Convert the inputs to a Dataset without labels.
    return tf.data.Dataset.from_tensor_slices(dict(features)).batch(batch_size)
# Here we just create an input_function that returns a dataset
# We don't give this input_function any labels because we are 
# not expected to have them 

features = ['SepalLength', 'SepalWidth', 'PetalLength', 'PetalWidth']
predict = {}

print("Please type numeric values as prompted.")
for feature in features:
  valid = True
  while valid:: 
    val = input(feature + ": ")
    if not val.isdigit(): valid = False
# The for-loop will loop through each key in the vector "features" 
# and will ask the user for the input to generate a prediction from
# the input vector "predict" 

  predict[feature] = [float(val)]

# Here we actually run the prediction 
predictions = classifier.predict(input_fn=lambda: input_fn(predict))

# Remember each prediction comes with different attributes, but the
# ones we are interested here are class_id (either of the 3 types 
# of flower) and probability for each class
for pred_dict in predictions:
    class_id = pred_dict['class_ids'][0]
    probability = pred_dict['probabilities'][class_id]
# Where class_id is the actual prediction (higher prob)
    print('Prediction is "{}" ({:.1f}%)'.format(
        SPECIES[class_id], 100 * probability))
```
