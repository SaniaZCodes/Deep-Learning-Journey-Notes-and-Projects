# 🧠 Handwritten Digit Recognition Using ANN

## 📌 Project Overview

This project demonstrates the implementation of an Artificial Neural Network (ANN) for handwritten digit recognition using the MNIST dataset.

The objective of the project is to classify handwritten digit images (0–9) by training a Neural Network using TensorFlow and Keras.

This project served as the first practical implementation of Deep Learning concepts including:

- Artificial Neural Networks (ANN)
- TensorFlow
- Keras
- Sequential API
- Dense Layers
- Activation Functions
- Optimizers
- Neural Network Training
- Model Evaluation

---

# 🎯 Problem Statement

Given an image of a handwritten digit, predict which digit (0–9) is present in the image.

### Input

```text
Handwritten Digit Image
(28 × 28 pixels)
```

### Output

```text
Digit Class

0,1,2,3,4,5,6,7,8,9
```

---

# 📊 Dataset Information

Dataset:

```text
MNIST Handwritten Digits Dataset
```

### Dataset Characteristics

- 60,000 Training Images
- 10,000 Testing Images
- 10 Classes (Digits 0–9)
- Image Size: 28 × 28 pixels

### Classes

```text
0
1
2
3
4
5
6
7
8
9
```

---

# 🔍 Dataset Understanding

Each image contains:

```text
28 × 28 pixels
```

Each pixel initially contains values:

```text
0 → 255
```

representing grayscale intensity.

---

# ⚙️ Data Preprocessing

The following preprocessing steps were applied.

---

## 1. Normalization

Pixel values were converted from:

```text
0 → 255
```

to:

```text
0 → 1
```

Purpose:

✅ Faster learning

✅ Better optimization

✅ Improved Neural Network performance

---

## 2. Flattening

Original image shape:

```text
28 × 28
```

Flattened shape:

```text
784 Features
```

Purpose:

✅ Convert image into a vector

✅ Prepare input for ANN

---

# 🧠 Artificial Neural Network Architecture

Structure:

```text
Input Layer (784 Features)
          ↓

Hidden Layer 1 (128 Neurons)
          ↓

Hidden Layer 2 (64 Neurons)
          ↓

Output Layer (10 Neurons)
```

---

# 🔥 Activation Functions

### Hidden Layers

```text
ReLU
```

Used to introduce non-linearity.

---

### Output Layer

```text
Softmax
```

Used to generate probabilities for the ten digit classes.

---

# ⚙️ Model Compilation

### Optimizer

```text
Adam
```

Purpose:

✅ Efficient weight updates

✅ Faster convergence

---

### Loss Function

```text
Sparse Categorical Crossentropy
```

Reason:

The labels are integer values:

```text
0–9
```

instead of one-hot encoded vectors.

---

# 🚀 Model Training

### Parameters

```text
Epochs = 10

Batch Size = 32
```

### Training Process

```text
Forward Propagation
       ↓

Prediction
       ↓

Loss Calculation
       ↓

Backpropagation
       ↓

Weight Updates
       ↓

Improved Predictions
```

---

# 📊 Model Evaluation

### Test Accuracy

```text
97.7%
```

### Test Loss

```text
0.0943
```

---

# 🎯 Prediction Example

The trained Neural Network successfully identified unseen handwritten digit images.

Example:

```text
Actual Digit    = 7

Predicted Digit = 7
```

✅ Correct Prediction

---

# 🧠 Key Deep Learning Concepts Used

- TensorFlow
- Keras
- Sequential API
- Dense Layers
- ReLU Activation
- Softmax Activation
- Loss Functions
- Optimizers (Adam)
- Forward Propagation
- Backpropagation
- Gradient Descent
- Neural Network Evaluation

---

# ✅ Project Outcome

The ANN successfully learned from the MNIST dataset and achieved high classification accuracy on unseen handwritten digit images.

This project provided practical experience with building, training, evaluating, and using Artificial Neural Networks for image classification tasks.

---

# 🎓 What I Learned

Through this project, I learned:

✅ How to preprocess image data

✅ How to build an ANN using TensorFlow and Keras

✅ How hidden layers learn patterns

✅ How activation functions influence model behavior

✅ How Neural Networks learn through Forward Propagation and Backpropagation

✅ How to evaluate and test Deep Learning models

---

# 🏁 Conclusion

Handwritten Digit Recognition using ANN served as my first Deep Learning project and provided hands-on experience with Neural Networks.

The project demonstrated the complete Deep Learning workflow:

```text
Dataset
     ↓

Preprocessing
     ↓

ANN Construction
     ↓

Training
     ↓

Evaluation
     ↓

Prediction
```

and established a strong foundation for future Deep Learning topics such as CNNs, Transfer Learning, Computer Vision, and NLP.
