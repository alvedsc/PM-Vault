---
{"dg-publish":true,"permalink":"/cards/vanishing-gradients-in-rn-ns/"}
---

up:: [[Recurrent Neural Networks\|Recurrent Neural Networks]] 
x:: 
d:: c

This is better explained in [Long Short-Term Memory (LSTM), Clearly Explained](https://www.youtube.com/watch?v=YCzL96nL7j0).

When you have a very long sequence like:

- The *cat*, which ate this and that and more of this and more of that, *was* full.
- The *cats*, which ate this and that and more of this and more of that, *were* full.

In these cases, the algorithm needs to remember stuff that happened early in the sequence to complete parts far away in the future. Instead, parts of the sequence are heavily affected by stuff that happens near them and terrible memory for words that were written way before... 

RNNs don't handle this very well bc of the [[Cards/Vanishing Gradients in RNNs\|Vanishing Gradients in RNNs]]. 

Backpropagation does not propagate the error very well to the beginning of the sequence. It can explode or vanish them. 

Vanishing gradients tend to be more common and less difficult to determine. When getting exploding gradients you get (NaN) values. 

When you have exploding gradients, you can apply Gradient Clipping (Clipping the values to a MAX). Vanishing gradients are more complicated. We need to use more complex architecture. 
