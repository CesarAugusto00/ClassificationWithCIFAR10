# PyTorch CIFAR-10 Classifier Playground

Welcome!  
This repository is for practicing and experimenting with different neural network architectures using [PyTorch](https://pytorch.org/) on the [CIFAR-10](https://www.cs.toronto.edu/~kriz/cifar.html) dataset.

## 🚩 **Goals**

- Learn PyTorch basics through hands-on experimentation
- Start with a simple fully-connected neural network
- Progress to using convolutional neural networks (CNNs)
- Observe and compare how different architectures affect classification accuracy

## 📦 **Contents**

- `simple_nn.py` — Fully-connected (linear) neural network for CIFAR-10
- `cnn.py` — Basic convolutional neural network
- `experiments/` — Folder for further model experiments
- `utils.py` — Helper functions for data loading and training

## 📊 **Dataset**

- **CIFAR-10**: 60,000 32x32 color images in 10 classes (airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck)
- Dataset is automatically downloaded by PyTorch's `torchvision.datasets`

## 🚀 **Getting Started**

1. **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/pytorch-cifar-playground.git
    cd pytorch-cifar-playground
    ```

2. **Install requirements:**
    ```bash
    pip install torch torchvision matplotlib
    ```

3. **Run a model:**
    ```bash
    python simple_nn.py
    ```
    or try the convolutional version:
    ```bash
    python cnn.py
    ```

4. **Modify or add architectures:**  
   Experiment with different layers and models in `experiments/`!

## 📝 **Project Structure**


