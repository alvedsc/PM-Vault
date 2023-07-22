---
{"dg-publish":true,"permalink":"/cards/distributed-probability-of-danger/"}
---

up:: [[Cards/Machine Learning\|Machine Learning]] 
x:: 
d:: s

The idea here would be to find predictability of crime as a distributed probability in a map. This coud be based on proximity in space and time to other crimes. 

For this model, a [[Cards/Weights\|weight]]  determines how much the probability of an event dilutes over the euclidian distance. This [[Cards/Weights\|weight]] is another parameter of the learning algorithm. The pixel value that would determine this could be 
$$p_{1}(t,r)= w_{1}/r$$Where $p_{1} (x,y)$ is the distributed probability of the event given another event that occured at a distance $d_e$. The parameter $w_1$ is the [[Cards/Weights\|weight]] of the event. It is invariant in the model. 

To develop this model, it is important to understand the effect previous crimes have on the current event, as well as the spatial distribution. However, the spatial distribution is not entirely localized. [[Convolutional Neural Networks\|Convolutional Neural Networks]] might not be the best way to understand these phenomena. [[Recurrent Neural Networks\|Recurrent Neural Networks]] might work better but these networks are still not understood, and there are better ways to predict sequential data than [[Recurrent Neural Networks\|Recurrent Neural Networks]]. 

A [[Cards/Machine Learning\|Machine Learning]] model for this could be a table database with times and locations. from this data, month, location, distance, and time passed could be input data for the model. I would just need to find a data base with enough data (could be a criminal database) to train the model and present it. 