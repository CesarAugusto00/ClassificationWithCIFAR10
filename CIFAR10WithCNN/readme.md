# 🚀 CIFAR-10 Image Classification with Convolutional Neural Networks (CNN)

This project demonstrates image classification on the [CIFAR-10 dataset](https://www.cs.toronto.edu/~kriz/cifar.html) using a Convolutional Neural Network (CNN) implemented with PyTorch.

## Overview

Previously, a feedforward neural network (fully connected network) was used to classify CIFAR-10 images.  
In this version, we build a more powerful **Convolutional Neural Network (CNN)** to improve the model's ability to recognize patterns in images.

## Dataset

- **CIFAR-10:**  
  - 60,000 color images (32x32 pixels)
  - 10 classes: airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck

## Model Architecture

The network consists of two convolutional layers, followed by three fully connected layers:

```python
self.conv1 = nn.Conv2d(3, 6, 5)         # 1st Conv Layer: 3 input channels (RGB), 6 output channels, 5x5 kernel
self.pool = nn.MaxPool2d(2, 2)          # Max Pooling: 2x2 window
self.conv2 = nn.Conv2d(6, 16, 5)        # 2nd Conv Layer: 6 in, 16 out, 5x5 kernel

self.fc1 = nn.Linear(16 * 5 * 5, 120)   # Fully Connected Layer 1
self.fc2 = nn.Linear(120, 84)           # Fully Connected Layer 2
self.fc3 = nn.Linear(84, 10)            # Output Layer (10 classes)

## Results

With this CNN architecture, the model achieves approximately 52% accuracy on the CIFAR-10 test set after a few epochs of training.
