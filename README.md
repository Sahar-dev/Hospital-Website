# Mnist_digit
# MNIST Neural Network Model Documentation

This neural network model is designed to classify images of handwritten digits from the MNIST dataset. The model consists of two hidden layers, each with 512 units and a rectified linear unit (ReLU) activation function. Dropout with a rate of 0.2 is applied after each hidden layer to prevent overfitting. The output layer has 10 units with a softmax activation function, allowing the model to classify images into one of 10 digits.

## Layers

### Input layer
- Dense layer with 512 units and an input shape of (784,) (flattened 28x28 pixel MNIST images).

### Hidden layers
- Dense layer with 512 units and a ReLU activation function.
- Dropout layer with a dropout rate of 0.2.
- Dense layer with 512 units and a ReLU activation function.
- Dropout layer with a dropout rate of 0.2.

### Output layer
- Dense layer with 10 units and a softmax activation function.

## Parameters

### Activation Functions
- ReLU activation function is used in both hidden layers.
- Softmax activation function is used in the output layer.

### Dropout
- Dropout is applied after each hidden layer with a dropout rate of 0.2.

### Optimizer
- Adam optimizer is used with default learning rate.

### Loss Function
- Categorical cross-entropy loss function is used.

### Epochs and Batch Size
- The model is trained for 50 epochs with a batch size of 100.

## Performance
- The model is evaluated on the MNIST test set.
- The accuracy metric is used to measure the performance of the model.
