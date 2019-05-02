## Gokul Raghunandan, gokulraghunandan@gmail.com, Batch 6 

# Convolution

On a very fundamental level Convolution is actually mathematical function, but for the purpose neural networks it can be thought of as an operation that amplifies or carries forward the important feautures from the input (usually an image) while ignoring the unimportant feautures. As shown below there are three elements needed for a convolution operation. They are the __input image__, __feature detector__ and the __feature map__. The feauture detector here acts as a kind of filter and the feature map is the output.

![hello](https://sds-platform-private.s3-us-east-2.amazonaws.com/uploads/70_blog_image_3.png)



# FIlters/Kernels

Filters in CNNs are in many ways similar to Instagram filters that we apply on images. they are matrices that contain specific values or weights that can detect specific features when applied on an image. Different filters have different functions. An edge detection filter applied to an image will enhance the edges in the image, a blur filter will blur the image. You can see some common filters applied in the image below. A feature detector matrix _strides_ over the image matrix to get these results.

![](https://cdn-images-1.medium.com/max/800/1*uJpkfkm2Lr72mJtRaqoKZg.png)



# Epochs

An epoch in a neural network is very similar to an iteration in programming terms. One epoch is the event of running the  all training training data trough the neural network and updating all the weights. Usually multiple epochs are run to improve the accuracy of the model as running only one epoch may lead to underfitting and running too many epochs may lead to overfitting. So it is essential to find the optimal epochs and the optimal epochs vary for every case.



# Activation function

Neurons in our body either "fire" or not based on the input they receive and neurons are an example of how activation functions work. They take an input and provide a binary, linear or non-linear output. Som eof the common activation function are:

1. Sigmoid function with output range from 0 to 1
2. Linear function with range from -$infinity$ to +$infinity$
3. RELU (Rectified linear unit)
4. Softmax



# Receptive field

![](https://github.com/aashray18521/tut/blob/master/Session%201/Session%201_files/0.8y3e18blaxk.gif?raw=true)





Receptive field is a hyperparameter that tells us how much of the input is affecting a particular unit in the network.

It not only depends on the filter applied and the previous layer but also on the number of layers that are there between the unit and the input layer. For example in the above image the receptive field of a yellow unit is 3$*$3 =9, in the second layer a green unit has a receptive field of 5$*​$5= 25.





