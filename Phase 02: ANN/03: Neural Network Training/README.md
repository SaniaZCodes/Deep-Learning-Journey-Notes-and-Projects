# ⚙️ Neural Network Training

## 📌 Overview

Building a Neural Network is only the first step.

To make accurate predictions, the Neural Network must learn from data by identifying mistakes and continuously improving its weights.

This learning process involves:

- Optimizers
- Neural Network Training

Together, these concepts help Neural Networks improve their predictions over time.

---

# 🚀 Optimizers

## 🎯 What is an Optimizer?

An Optimizer is an algorithm that updates the weights of a Neural Network in order to reduce prediction errors and improve model performance.

### Simple Definition

```text
Optimizer

=

Weight Updating Algorithm
```

---

# 🧠 Why Do We Need Optimizers?

After Backpropagation identifies errors, the Neural Network must update its weights.

Optimizers perform these updates and help the model move toward lower loss and better predictions.

---

# 🔄 Learning Process

```text
Prediction
      ↓

Loss Function
      ↓

Error
      ↓

Backpropagation
      ↓

Gradients
      ↓

Optimizer
      ↓

Weight Update
```

---

# 🚗 Navigation Analogy

Imagine traveling to a destination.

### Gradient

```text
Shows Direction
```

### Optimizer

```text
Controls Movement
```

The optimizer decides how the model should move toward a better solution.

---

# 🌟 Popular Optimizers

## SGD (Stochastic Gradient Descent)

Simple and traditional optimizer.

Characteristics:

✅ Easy to understand

✅ Updates weights step by step

❌ Can be slower in some situations

---

## Adam

Most commonly used optimizer.

Characteristics:

✅ Fast

✅ Stable

✅ Efficient

✅ Works well for most Deep Learning projects

---

## RMSProp

Another popular optimizer.

Characteristics:

✅ Adaptive learning behavior

✅ Commonly used in Deep Learning applications

---

# 🎯 Most Common Beginner Choice

For many ANN projects:

```python
optimizer="adam"
```

Adam is usually the default choice because it performs well in most situations.

---

# ✅ Key Points

- Optimizers update neural network weights.
- Reduce loss and improve predictions.
- Use gradients generated during backpropagation.
- Adam is the most widely used optimizer.
- Different optimizers use different update strategies.

---

# 🚀 Neural Network Training

## 🎯 What is Training?

Training is the process in which a Neural Network learns patterns from data by repeatedly making predictions and correcting mistakes.

### Simple Definition

```text
Training

=

Learning From Data
```

---

# 🧠 Why Do We Need Training?

Initially, Neural Networks know nothing about the data.

During training, the model gradually learns patterns and improves its predictions.

---

# 🔄 Complete Training Cycle

```text
Input Data
      ↓

Forward Propagation
      ↓

Prediction
      ↓

Loss Function
      ↓

Error
      ↓

Backpropagation
      ↓

Optimizer
      ↓

Weight Update
      ↓

Better Prediction
```

This cycle repeats many times until the model learns.

---

# 📈 Training Goal

The main objectives of training are:

✅ Reduce Loss

✅ Improve Accuracy

✅ Learn Patterns From Data

---

# 🎯 Epoch

An Epoch is one complete pass through the entire training dataset.

### Example

Dataset:

```text
1000 Images
```

If the model sees all images once:

```text
1 Epoch
```

If the model sees all images again:

```text
2 Epochs
```

And so on.

---

# 🎯 Batch

A Batch is a small subset of the training data used during learning.

### Example

Dataset:

```text
1000 Images
```

Batch Size:

```text
32
```

The model learns from:

```text
32 Images
```

at a time.

---

# 📚 Epoch vs Batch

### Epoch

```text
Complete Dataset
```

---

### Batch

```text
Small Portion Of Dataset
```

---

# 💻 Training Example

```python
model.fit(
    X_train,
    y_train,
    epochs=10,
    batch_size=32
)
```

Meaning:

```text
Train Model
For 10 Epochs
Using Batches Of 32 Samples
```

---

# ✅ Key Points

- Training is the learning process of a Neural Network.
- Training improves model performance over time.
- Epoch = one complete pass through the dataset.
- Batch = small subset of the dataset.
- Training repeatedly updates weights to reduce loss.
- The goal is to produce better predictions.

---

# 🎓 Interview Questions

### What is an Optimizer?

An Optimizer is an algorithm used to update the weights of a Neural Network in order to reduce loss and improve performance.

---

### What is Training in Deep Learning?

Training is the process of repeatedly making predictions, calculating errors, and updating weights so that the Neural Network can learn from data.

---

### What is an Epoch?

An Epoch is one complete pass through the entire training dataset.

---

### What is a Batch?

A Batch is a small subset of the training data used during one learning step.

---

### Which Optimizer is most commonly used?

Adam is one of the most widely used optimizers in Deep Learning.

---

# 🌟 Memory Tricks

## Optimizer

```text
Find Error
      ↓
Update Weights
      
