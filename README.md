# Image-Classification-using-MNIST-Digits
This project is based on detecting handwritten images of numbers. The data set that has been used is Mnist data set which is built in data set available in tensorflow library.
# Introduction: 
### This project is based on detecting handwritten images of numbers. The data set that has been used is Mnist data set which is built in data set available in tensorflow library (Abadi et al. 2016). The reason of the study is to detect handwritten digits as well as to compare different models with different activation functions. However, detecting all the provided inputs correctly is not the goal here.
### In the models two different models have been used. The first model is uses ReLu as the activation function whearase the second one uses TanH with the final activation layer of both the models as ‘softmax’. Further details regarding the models are discussed in the methodology section
# Model Architecture
### There are two different models as follows:
## Model_1:
#### The first model comprises of one input layer, one hidden layer which is ReLu and an output layer with 10 nodes and uses ‘softmax’ as its activation function. The number of inputs in the first layer is 784 as these are the number of pixels in one image of the data set. The hidden layer consists of 256 nodes and the output layer has 10 nodes as the number of possible outcomes are 10 ranging from 0 to 9.
## Model_2:
#### The second model comprises of one input layer, one hidden layer which is TanH and an output layer with 10 nodes and uses ‘softmax’ as its activation function. The number of inputs in the first layer is 784 as these are the number of pixels in one image of the data set. The hidden layer consists of 256 nodes and the output layer has 10 neurons as the number of possible outcomes are 10 ranging from 0 to 9. 
# Training Process
### Several factors which take part in the training procedure are optimizer, learning_rate, loss_function, activation_function, No. of Epochs, Batch_size, no. of neurons inside of each layer. 
1.	Optimizer: 	Adam
2.	Learning Rate:	 0.1% (0.001)
3.	Loss Function:	 Categorical_Crossentropy
4.	Activation Function: Model_1/ Relu and Model_2/ Tanh
5.	Epochs: 	Scenario_1:- 25 ; Scenario_2:- 10
6.	Batch Size: 	Scenario_1:- 32 ; Scenario_2:-10
7.	Number of Neurons: 
a)	Hidden Layer: 	256
b)	Output Layer: 	10
# Evaluation:
### The models have been evaluated using the testing data set. The factors taken into account are accuracy and loss achieved after several number of epochs. In order to understand them better, a graph of accuracy against loss during epochs has been plotted, results of which have been elaborated in next sections.
# Conclusion
### The ReLU-based model outperforms the Tanh-based model for the MNIST data set in terms of loss minimization, accuracy, and stability, making it a more efficient choice for this classification task. However, the differences are not drastic, and both models achieve strong overall performance.
