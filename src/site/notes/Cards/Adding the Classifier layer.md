---
{"dg-publish":true,"permalink":"/cards/adding-the-classifier-layer/"}
---

up:: [[Cards/Performing transfer learning in tensorflow\|Performing transfer learning in tensorflow]] 
x:: 
d:: p

Objective: To build our classifier layer. 

First is the layer previous to the classification. It is a [[Fully Connected\|Fully Connected]] layer. This process is simply a [[Flatten\|Flattening]]. For reasons I still don't understand, the course used the following, instead of flatten()

```
global_average_layer = tf.keras.layers.GlobalAveragePooling2D()
```

And then, this [[Fully Connected\|Fully Connected]] layer is transformed into the single neuron, using the following code

```
prediction_layer = keras.layers.Dense(1)
```

Finally, we add these two layers to the model

```python
model = tf.keras.Sequential([
  base_model,
  global_average_layer,
  prediction_layer
])
```

Take a look at the output of model.summary()

```
Model: "sequential_1"
_________________________________________________________________
 Layer (type)                Output Shape              Param #   
=================================================================
 mobilenetv2_1.00_160 (Funct  (None, 5, 5, 1280)       2257984   
 ional)                                                          
                                                                 
 global_average_pooling2d (G  (None, 1280)             0         
 lobalAveragePooling2D)                                          
                                                                 
 dense (Dense)               (None, 1)                 1281      
                                                                 
=================================================================
Total params: 2,259,265
Trainable params: 1,281
Non-trainable params: 2,257,984
_________________________________________________________________
```

Notice the following:
- the global_average_pooling2d is an average pooling of 5 x 5 size
- the Dense layer has 1281 parameters: 
	- 1280 weights for each [[Node\|neuron]] 
	- 1 [[Biases\|bias]] 