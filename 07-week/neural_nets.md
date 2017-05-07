# Neural Networks
-----

## Structure of Neural Network
- modeling technique that takes advantage of using our input data, transforming that data based on some *weights* of the importance of our features into **hidden layers** that combines and analyzes the relationship of our hidden layer using weights of our data to provide an *output*
- must have: **input**, **output**, **hidden layer** that connects those things

Contrast linear regression: LR assumes linearity between input and output, errors are independent for all X

The weights of a neural network are comparable to the beta values of a linear regression

Single-layer NNs are called "perceptrons" 

**Epoch** - a full training run across all of our data



## Capturing Relationships in Data
- the purpose of the hidden layer is to apply a function to the interactions of our input variables -- this is called an **activation function**
- to find weights:

## Coding a Neural Network
- start by coding a numpy array of the number of input nodes and associated weights
- for a 2-input network with one hidden layer, you need 6 weights
