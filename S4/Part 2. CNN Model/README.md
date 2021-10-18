**Problem Statement**

Train the MNIST dataset under the following restrictions

99.4% validation accuracy
Less than 20k Parameters
You can use anything from above you want.
Less than 20 Epochs
Have used BN, Dropout, a Fully connected layer, have used GAP.


**Solution**

A model was trained with 19,678 parameters and 99.56% test accuracy.

Model parameters
Number of layers: 7 Convolution Layers, 2 Transition Layers

Batch Size: 64 Optimizer: SGD Loss Function: NLL Loss

**Model Architecture**

12->24->36->MP->12->12->24->MP->12->12->24->GAP(7x7)->Dense-> 10 outputs
