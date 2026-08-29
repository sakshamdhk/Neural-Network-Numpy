# Neural Network from Scratch - MNIST Digit Recognition (NumPy)

A feedforward neural network built entirely from scratch using NumPy to classify handwritten digits from the MNIST dataset.

## Overview

This project implements the full training pipeline of a neural network manually, including forward propagation, backpropagation, and gradient descent, to understand exactly what deep learning frameworks abstract away.

**Test accuracy achieved: ~91%**

## What's implemented

- Forward propagation through a multi-layer network
- ReLU activation for hidden layers
- Softmax activation for the output layer
- Cross-entropy loss
- Backpropagation (manual gradient derivation and implementation)
- Gradient descent parameter updates
- Training/test accuracy visualization

## Why from scratch
This was built to understand the actual mechanics underneath: how gradients flow backward through a network, how weight updates are derived, and why the standard architectural choices (ReLU, softmax, cross-entropy) work the way they do together.

## Dataset

Uses the [MNIST dataset](http://yann.lecun.com/exdb/mnist/) of handwritten digits (28x28 grayscale images, 10 classes).

The dataset files are **not included** in this repo (excluded via `.gitignore` due to size). To run this project:

1. Download the MNIST dataset (CSV format) — e.g. from [Kaggle](https://www.kaggle.com/datasets/oddrationale/mnist-in-csv)
2. Place `mnist_train.csv` and `mnist_test.csv` in the project directory
3. Run the training script

## Requirements

```bash
pip install numpy matplotlib
```


## Architecture

- **Input layer:** 784 neurons (28x28 flattened pixel values)
- **Hidden layer(s):** ReLU activation
- **Output layer:** 10 neurons (digit classes 0–9), softmax activation
- **Loss function:** Cross-entropy
- **Optimization:** Gradient descent

## Results

The model achieves approximately 91% accuracy on the MNIST test set after training.

## Author

[Shaksham](https://github.com/sakshamdhk)
