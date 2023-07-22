---
{"dg-publish":true,"permalink":"/cards/deep-rn-ns/"}
---

up:: [[Recurrent Neural Networks\|Recurrent Neural Networks]] 
x:: [[Bidirectional RNN\|Bidirectional RNN]] 
d:: c

For more complex functions, you might need to stack various layers of RNNs

One layer of an RNN looks like this:

![[Deep RNNs.20-02-2023-1.png\|Deep RNNs.20-02-2023-1.png]]

To generalize this to any RNN of any depth, we can stack hidden layers of the network as follows:

![[Deep RNNs.20-02-2023-3.png\|Deep RNNs.20-02-2023-3.png]]

Where
- each activation function has the format $a^{[l]<t>}$ 
- the index $l$ corresponds to each layer in the network

For example, the value of $a^{[2]<3>}= g(W_{a}^{[2]}[a^{[2]<2>},a^{[1]<3>}]+b_{a}^{[2]})$ 
Where
- g is the activation function

The activation blocks can also be [[Recurrent Neural Networks\|Recurrent Neural Networks]] , [[Gated Recurrent Unit\|Gated Recurrent Unit]]  or [[Long-Short-Term Memory\|Long-Short-Term Memory]] blocks. Also, the concept of [[Bidirectional RNN\|Bidirectional RNN]] can be employed here too. 

Another architecture that is being used is not using very deep RNNs, but stacking several hidden layers between the output of the last RNN and the $\hat{y}$ , as follows (observe the squares on the top):

![[Deep RNNs.20-02-2023-4.png\|Deep RNNs.20-02-2023-4.png]]

Very [[Cards/Deep RNNs\|Deep RNNs]] are not very common because they require a lot of computational power. 

