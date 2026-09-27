# 🏗️ Building Neural Networks

## 📌 Overview

Before training a Neural Network, we must first build its structure.

In Keras, Neural Networks are commonly created using:

- Sequential API
- Dense Layers

These components allow us to define how data flows through the network and how neurons are organized.

---

# 🚀 Sequential API

## 🎯 What is Sequential API?

Sequential API is the simplest way to create a Neural Network in Keras.

The word:

```text
Sequential
```

means:

```text
One Layer After Another
```

Data moves through the network in a linear sequence.

---

# 🧠 Basic Structure

```text
Input Layer
      ↓

Hidden Layer
      ↓

Output Layer
```

Each layer is connected in order.

---

# 💻 Creating a Sequential Model

```python
from tensorflow.keras.models import Sequential

model = Sequential()
```

This creates an empty Neural Network.

Layers can then be added one by one.

---

# 🎯 Why Use Sequential API?

Sequential API is:

✅ Beginner Friendly

✅ Easy to Understand

✅ Ideal for ANN Models

✅ Easy to Maintain

---

# 🌟 Real World Analogy

Imagine a pipeline:

```text
Input
  ↓

Step 1
  ↓

Step 2
  ↓

Step 3
  ↓

Output
```

Everything happens in sequence.

This is exactly how a Sequential Model works.

---

# 🚀 Dense Layers

## 🎯 What is a Dense Layer?

A Dense Layer is a neural network layer where every neuron is connected to every neuron in the next layer.

These connections allow the network to learn patterns from data.

---

# 🧠 Dense Layer Intuition

Suppose we have:

```text
Age
Income
CGPA
```

as inputs.

A Dense Layer learns relationships between these features and helps the network make predictions.

---

# 💻 Creating a Dense Layer

Example:

```python
Dense(10)
```

Meaning:

```text
A Dense Layer
with 10 Neurons
```

---

# Example

```python
model.add(Dense(10))
```

This adds a Dense Layer containing 10 neurons to the Neural Network.

---

# 🎯 Why Dense Layers Are Important

Dense Layers:

✅ Learn feature relationships

✅ Perform calculations

✅ Extract useful patterns

✅ Generate meaningful representations of data

---

# 🏗️ ANN Structure Example

```text
Input Layer
      ↓

Dense Layer (10 Neurons)
      ↓

Dense Layer (5 Neurons)
      ↓

Output Layer (1 Neuron)
```

This is a simple Artificial Neural Network (ANN).

---

# 🔗 Relationship Between Sequential API and Dense Layers

Sequential API provides:

```text
Neural Network Structure
```

Dense Layers provide:

```text
Neurons Inside That Structure
```

---

# 🚀 Building a Neural Network

```text
Sequential Model
       ↓

Add Dense Layer
       ↓

Add Another Dense Layer
       ↓

Add Output Layer
       ↓

Neural Network Ready
```

---

# ✅ Key Points

### Sequential API

- Simplest way to create Neural Networks.
- Layers are added one after another.
- Ideal for ANN models.
- Easy to understand and use.

### Dense Layers

- Contain neurons.
- Every neuron connects to every neuron in the next layer.
- Learn relationships and patterns in data.
- Commonly used in Artificial Neural Networks.

---

# 🎓 Interview Questions

### What is Sequential API?

Sequential API is a Keras API that allows developers to build Neural Networks layer by layer in a linear sequence.

---

### What is a Dense Layer?

A Dense Layer is a neural network layer where every neuron is connected to every neuron in the next layer.

---

### Why are Dense Layers important?

Dense Layers help Neural Networks learn patterns and relationships from data.

---

# 🌟 Memory Trick

```text
Sequential API
       ↓
Neural Network Structure

Dense Layers
       ↓
Neurons Inside Structure
```

---

# 🏁 Conclusion

Sequential API and Dense Layers are fundamental building blocks of Artificial Neural Networks. Sequential API defines how layers are arranged, while Dense Layers provide the neurons that learn patterns from data. Together they form the foundation of ANN development in Keras.
