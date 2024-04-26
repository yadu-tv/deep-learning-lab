# Deep Learning

## Note:

* Wherever possible, draw diagrams
* Give examples everywhere

## Module 1 - Introduction to neural networks and deep neural network

### Theory
* Difference between ML and DL
* Explanation with respect to fully connected NN
* Design a fully connected NN
  * Calculate parameters
  * Input of a layer
  * Output of a layer
* Explaination of a graph/model/diagram


### Numericals
* Forward propogation
  * a. Sigmoid function
  * b. Relu function
* Back propogation
  * a. Weights
  * b. Weights and Biases
* Multi Layer Perceptron
  * Realizaation of gates, SOP, POS
* Activation function analysis

## Module 2 - Convolution Neural Networks

### Theory
* Why use ALexNet (Skip connections), ResNet(Learning proglem - Exploding/Vanishing gradient), GoogleNet (1x1 filter), VGG16 (Also has 1x1 filter) ?
  * If skip = 3 => More accuracy
  * If skip = 20 => Less accuracy
* Choosing which pretrained model is best for a given situation?
* Calculating number of tasks when dimensions are reduced? (GoogleNet has very less number of tasks compared to VGG16)
* What is Inception module in GoogleNet?
* GoogleNet can produce results in each steps rather than waiitng for the model to finish.

### Numericals
* What is convolution - Filter, kernel, Pooling (Max, Min and Avg)?
* Performing calculations to find output dimension when passed through different filter sizes
* Make sure to include filters in the output layers
* Work on 4 and even 5 dimensions

## Module 3 - Improving deep neural networks

### Theory
* Gradient Descent/Stochastic Gradient Descent/Batch Stochastic Gradient Descent
* Choosing the best regularization
* Choosing the best normalization method
* Optimization functions like ADAM, ADAGRAD, RMSPROP
* Validation, Cross Validation, How we sample the data
* Data augmentation
* Weight initialization
  * Functions like TanH, Sigmoid - Xavier, ReLu - Heap (Downsides of these functions)
  * Identifing the values if 3 different cost functions are given
    * C1 - 0.9; 0.91; 0.92; 0.89; 0.89
    * C2 - 0.9; 0.7; 0.5; 0.4; 0.2
    * C3 - 0.9; 0.8; 0.77; 0.72; 0.6
    * ReLu - Heap works best in C2
    * When values are swapped, then Sigmoid on C3 works the best
* Autotuning
* Batch normalization

### Numericals
* Optimisation of a function (usually single variable)
* Regularization (Loss functions)
  * L1
  * L2
  * Cross Entropy (including softmax)
* Optimization using functions like ADAM, Momentum, ADAGRAD, RMSPROP

## Module 4 - Recurrent networks

### Theory
* If application is spatial - CNN
* If application is temporal (with respect to time) - RNN, LSTM
* Basic RNN structure - including multiple layers
* Weights do not change in this case as it is recurrent
* Calculating number of newrons
  * x nuerons
  * n number of unrolls
  * total neurons = x*n
  * number of parameters = n*3

### Lab