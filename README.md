# UE24CS645BC2_-PES1PG25CS077-_Fashion_MNIST_CNN



# Fashion MNIST CNN From Scratch

## Assignment Overview

This assignment implements a Convolutional Neural Network (CNN) completely from scratch using only NumPy using basic principles.

The objective of this assignment is to understand the internal working of CNNs by manually implementing:
- Convolution Layer
- MaxPooling Layer
- Flatten Layer
- Fully Connected Layer
- Forward Propagation
- Backpropagation
- Gradient Descent Weight Updates

The model is trained and evaluated on the Fashion-MNIST dataset.

---

# Dataset

Dataset Used:
- Fashion-MNIST

The dataset contains:
- 70,000 grayscale images
- 10 clothing categories
- Image size: 28 × 28

Dataset Link:
https://www.kaggle.com/datasets/oddrationale/mnist-in-csv

Files used:
- fashion-mnist_train.csv
- fashion-mnist_test.csv

---

# CNN Architecture

Input Image (28×28)
↓
Convolution Layer
↓
ReLU Activation
↓
MaxPooling Layer
↓
Flatten Layer
↓
Fully Connected Layer
↓
ReLU Activation
↓
Output Layer
↓
Softmax

---

# Features Implemented

## Convolution Layer
- Manual convolution operation
- Forward propagation
- Backpropagation

## MaxPooling Layer
- Forward pooling
- Gradient routing during backward pass

## Activation Function
- ReLU activation

## Fully Connected Layer
- Dense layer implementation
- Weight and bias updates

## Loss Function
- Softmax Cross Entropy Loss

## Training Pipeline
- Forward pass
- Loss computation
- Backward pass
- Gradient descent updates

---

# Training Details

Due to the computational complexity of implementing CNN operations manually using nested Python loops, training was performed on a subset of the Fashion-MNIST dataset.

Training Configuration:
- Training Samples: 1000
- Testing Samples: 500
- Epochs: 3
- Batch Size: 5
- Learning Rate: 0.001

Training Process:
1. Images are normalized to the range [0,1]
2. Images pass through convolution and pooling layers
3. Features are flattened
4. Fully connected layers generate class scores
5. Softmax computes probabilities
6. Cross entropy loss is calculated
7. Backpropagation updates weights and biases

---

# Testing and Evaluation

The trained model was evaluated on a subset of the test dataset.

Evaluation Metrics:
- Test Accuracy
- Prediction Visualization
- Loss Reduction During Training

Observed Results:
- The loss decreases during training, indicating successful learning.
- Since the implementation is fully manual and uses a small training subset, accuracy is lower compared to optimized deep learning frameworks.
- The primary goal of this assignment is understanding of CNN internals rather than achieving state-of-the-art performance.

---

# Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Jupyter Notebook

---

# How to Run

## Install Required Libraries

```bash
pip install numpy pandas matplotlib scikit-learn notebook
```

## Start Jupyter Notebook

```bash
python -m notebook
```

## Open Notebook

Open:
```text
Fashion_MNIST_CNN.ipynb
```

Run all cells.

---

# Project Structure

```text
project/
│
├── Fashion_MNIST_CNN.ipynb
├── README.md
├── fashion-mnist_train.csv
└── fashion-mnist_test.csv
```

---

# Notes

- The CNN is implemented completely from scratch without using deep learning frameworks like TensorFlow or PyTorch.
- All forward and backward propagation logic is manually implemented using NumPy.
- Pure Python nested loops make convolution operations computationally expensive.
- Therefore, a reduced dataset subset was used for practical execution time on CPU.

---

# Author

Name: BASAVAPRABHU S

USN: PES1PG25CS077
