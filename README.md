# NUARAL## 📌 Project Overview
This project implements a Multilayer Perceptron (MLP) using PyTorch as part of a Neural Networks course.

The goal is to perform image classification on the Fashion-MNIST dataset, which contains grayscale images of clothing items belonging to 10 different classes.

Two different experiments were conducted by modifying the learning rate and the number of hidden layers to analyze their effect on model performance.

---

## 📊 Dataset Description
The Fashion-MNIST dataset is used in this project. It consists of:
- 60,000 training images
- 10,000 test images
- 10 classes of clothing items
- Image size: 28x28 grayscale

The dataset is loaded using torchvision and split into training, validation, and testing sets.

---

## ⚙️ Data Preprocessing
The following preprocessing steps were applied:
- Conversion of images to tensors
- Normalization to stabilize training
- Splitting training data into training and validation sets (80/20 split)

---

## 🧠 Model Architecture

### Experiment 1
- Input layer: Flatten (28x28 = 784 features)
- Hidden layers: 2 fully connected layers (256, 128 neurons)
- Activation function: ReLU
- Regularization:
  - Batch Normalization
  - Dropout (0.3)
- Output layer: 10 neurons (classification classes)
- Learning rate: 0.001

### Experiment 2
- Input layer: Flatten layer
- Hidden layers: 3 fully connected layers (512, 256, 128 neurons)
- Activation function: ReLU
- Regularization:
  - Batch Normalization
  - Dropout (0.3 / 0.2)
- Output layer: 10 neurons
- Learning rate: 0.0001

---

## 🏋️ Training Process
The model was trained using:
- Optimizer: Adam
- Loss function: CrossEntropyLoss
- Number of epochs: 10
- Batch size: 64

During training, both loss and accuracy were monitored for:
- Training set
- Validation set

---

## 🔬 Experiments Summary
Two experiments were conducted:
- Experiment 1: Baseline model with 2 hidden layers and LR = 0.001
- Experiment 2: Deeper model with 3 hidden layers and LR = 0.0001

---

## 📈 Results
Both models achieved strong performance on the dataset:
- Accuracy range: ~88% – 89%
- Experiment 2 showed slightly better generalization on validation and test sets.

---

## 📊 Visualizations
The following plots were included:
- Training vs Validation Loss curves
- Training vs Validation Accuracy curves
- Comparison between both experiments

---

## 🧪 Regularization Techniques
To improve generalization and reduce overfitting, the following techniques were applied:
- Dropout layers
- Batch Normalization

---

## 🚀 How to Run
Install dependencies:
```bash
pip install torch torchvision matplotlib pandas



📌 Notes

This project is implemented using PyTorch and follows a standard neural network pipeline including training, validation, and evaluation phases
