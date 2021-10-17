**Neural Network**

This exercise is primarily focused on understanding the math and logic behind how a neural network works. Solved with a simple 2 layer Fully connected layer network. In this exercise, we will look at how forward propagation works, how loss is calculated for different problem objectives, how we perform back propagation to update the weights (learning process) and finally how learning rate plays a role in weights update.

**Network Architecture**

The architecture used for example problem solved is a regression problem with architecture consisting of 2 hidden layers and 2 neurons per hidden layer.

**Steps for Forward propagation:**

The following steps are also relevant if we had many more hidden layers (deep) as well as many more neurons in each of the hidden layer. This example shows only 2 hidden layer and 2 neurons per layer.

First hidden layer: the inputs i1, i2 are multiplied with weights (w1, w2, w3, s4) to form the first hidden layer (2 neurons h1 & h2) - Refer to hidden-1 calculations below

Activation: since h1, h2 are in linear form, activation function is applied to get outputs a_h1, a_h2. While the most common is relu, in this example sigmoid activation is applied. (some of activation functions : relu, sigmoid, or tanh)

Second hidden layer: the outputs of activations from first hidden layer (a_h1, a_h2) is then further multiplied (sum product) to formulate the hidden layer -2. The outputs is represented as o1, o2. Similar to first layer, an activation is applied to o1 & o2 represented by a_o1, a_o2. Refer to hidden-2 calculation below

Error: The outputs of the neurons a_o1, a_o2 is compared with the actual inputs (i1, i2). The representation of this comparison is shown as errors (E1, E2) which shows how far off we are from the real data. There are multiple ways to represent the error, the the most common form are shown below and figure

​ Mean Square Error for regression problem

​ cross entropy loss for a classification problem

Total Error (Total Loss): Now that we have errors from individual data, they are summed up to arrive at the total loss.

**Steps for Backward propagation:**

1. Intialize weight randomly
2. Loop untill convergence
    a. Compute Gradient
    b. Update Weights
3. Return Weights
