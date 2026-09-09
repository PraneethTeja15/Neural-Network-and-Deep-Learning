# Neural-Network-and-Deep-Learning
Python implementation for CS5720 Home Assignment 1 covering TensorFlow tensor manipulation, loss functions, optimizer comparison, and TensorBoard.
This repository contains the Python code for the programming section of CS5720: Neural Network and Deep Learning – Home Assignment 1.

Requirements
Python 3.x
TensorFlow
NumPy
Matplotlib

Install the required packages using:

pip install tensorflow numpy matplotlib
How to Run

Open the project in VS Code and run:

python CS5720_Home_Assignment_1_code.py

The program performs all four programming tasks.

1. Tensor Manipulations and Reshaping

This section demonstrates basic TensorFlow tensor operations.

It includes:

Creating a random tensor with shape (4, 6)
Finding the rank and shape of the tensor
Reshaping the tensor to (2, 3, 4)
Transposing the tensor to (3, 2, 4)
Creating a smaller (1, 4) tensor
Using TensorFlow broadcasting to add the smaller tensor to another tensor

The program prints the tensor rank and shapes before and after the transformations.

2. Loss Functions and Hyperparameter Tuning

This section demonstrates two commonly used loss functions:

Mean Squared Error (MSE)
Categorical Cross-Entropy (CCE)

The program:

Defines true labels and predicted values.
Calculates the MSE and CCE losses.
Slightly changes the predictions.
Calculates the losses again.
Compares the loss values using a bar chart.

The generated chart is saved as:

loss_comparison.png
3. Training a Model with Different Optimizers

This section uses the MNIST handwritten digit dataset to compare two optimizers:

Adam
SGD

The program:

Loads the MNIST dataset.
Normalizes the image values.
Builds a simple neural network.
Trains one model using Adam.
Trains another model using SGD.
Compares their training and validation accuracy.

The accuracy comparison is saved as:

adam_vs_sgd_accuracy.png
4. TensorBoard

This section demonstrates how TensorBoard can be used to monitor model training.

The program:

Loads and preprocesses the MNIST dataset.
Builds a simple neural network.
Trains the model for 5 epochs.
Records training information using TensorBoard.
Saves training and validation accuracy and loss plots.

TensorBoard log files are stored in:

logs/fit/

To launch TensorBoard, run:

tensorboard --logdir logs/fit

Then open the local TensorBoard address shown in the terminal.

Output Files

After running the program, the following files may be generated:

loss_comparison.png
adam_vs_sgd_accuracy.png
tensorboard_accuracy.png
tensorboard_loss.png
logs/fit/
