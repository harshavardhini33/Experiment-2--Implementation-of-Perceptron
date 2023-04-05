# Experiment-2--Implementation-of-Perceptron
##AIM:

To implement a perceptron for classification using Python

## EQUIPMENTS REQUIRED:
Hardware – PCs
Anaconda – Python 3.7 Installation / Google Colab /Jupiter Notebook

## RELATED THEORETICAL CONCEPT:
* A Perceptron is a basic learning algorithm invented in 1959 by Frank Rosenblatt. It is meant to mimic the working logic of a biological neuron. The human brain is basically a collection of many interconnected neurons. Each one receives a set of inputs, applies some sort of computation on them and propagates the result to other neurons.
* A Perceptron is an algorithm used for supervised learning of binary classifiers.Given a sample, the neuron classifies it by assigning a weight to its features. To accomplish this a Perceptron undergoes two phases: training and testing. During training phase weights are initialized to an arbitrary value. Perceptron is then asked to evaluate a sample and compare its decision with the actual class of the sample.If the algorithm chose the wrong class weights are adjusted to better match that particular sample. This process is repeated over and over to finely optimize the biases. After that, the algorithm is ready to be tested against a new set of completely unknown samples to evaluate if the trained model is general enough to cope with real-world samples.
* The important Key points to be focused to implement a perceptron:
* Models have to be trained with a high number of already classified samples. It is difficult to know a priori this number: a few dozen may be enough in very simple cases while in others thousands or more are needed.
* Data is almost never perfect: a preprocessing phase has to take care of missing features, uncorrelated data and, as we are going to see soon, scaling.
* Perceptron requires linearly separable samples to achieve convergence.

## The math of Perceptron
* If we represent samples as vectors of size n, where ‘n’ is the number of its features, a Perceptron can be modeled through the composition of two functions. The first one 
f(x) maps the input features  ‘x’  vector to a scalar value, shifted by a bias ‘b’
![formula2](https://user-images.githubusercontent.com/93427208/229996763-131971c3-e302-45c8-aef6-f5d4a544e5a0.png)

* A threshold function, usually Heaviside or sign functions, maps the scalar value to a binary output:
![formula1](https://user-images.githubusercontent.com/93427208/229996776-f7f2abff-b57c-4848-8d48-f0836655197c.png)
* Indeed if the neuron output is exactly zero it cannot be assumed that the sample belongs to the first sample since it lies on the boundary between the two classes. Nonetheless for the sake of simplicity,ignore this situation.


## ALGORITHM:
1. Importing the libraries
2. Importing the dataset
3. Plot the data to verify the linear separable dataset and consider only two classes
4. Convert the data set to scale the data to uniform range by using Feature scaling
![formula3](https://user-images.githubusercontent.com/93427208/229996912-34ff2bbf-7dcb-45ed-aa2b-13e473f2709e.png)

5. Split the dataset for training and testing
6. Define the input vector ‘X’ from the training dataset
7. Define the desired output vector ‘Y’ scaled to +1 or -1 for two classes C1 and C2
8. Assign Initial Weight vector ‘W’ as 0 as the dimension of ‘X’
9. Assign the learning rate
10. For ‘N ‘ iterations ,do the following:
        ![formula4](https://user-images.githubusercontent.com/93427208/229997015-fd5ec7a8-3788-461b-aae9-2858d1042bc7.png)

11. Plot the error for each iteration 
12. Print the accuracy


 ## PROGRAM:
