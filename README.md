## MNIST handwriting recognition
Using MNIST handwriting images dataset to train neural network handwriting recognition model (1st model)
- "data.zip" contains both training data and test data for training model and compute the performance of model
- "data_my_model.zip" contains some particular random handwriten images which is used to check the model optionally

28\*28 images are considered as input to neural network model with 3 layers (Input layer: 784 nodes (28\*28); 1 hidden layer: 100 nodes; output layer: 10 node (represent number from 1 to 10)). I also use backpropagation technique and sigmoid function as activation function for this model


![](https://i2.wp.com/syncedreview.com/wp-content/uploads/2019/06/MNIST.png?fit=530%2C297&ssl=1)

## Neural network Rotation Backquery
The 2nd model also uses 3-layer neural network and the purpose of it is to recover the (28\*28) image from the set of output layer using "Backquery" technique AND the inverse of sigmoid function (inverse activation function)
- Input: the list of 10 units as the output layer of the original handwriting recognition project
- Output: (28\*28) image 
- "Rotation" technique is used to improve the performance of the model by rotating the image to +/- 10 degrees
- "Scaling" technique: scale the input to between 0.01 and 1 (It's a must to avoid 0 value -> Can harm the performance of model)

(Model must be trained as normal before performing "Backquery" technique) AND Through this way, we'll have an intuition of how the model learn from data to ouput the result
