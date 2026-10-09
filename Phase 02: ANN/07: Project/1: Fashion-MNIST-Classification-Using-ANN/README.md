# 👕 Fashion Product Classification Using Artificial Neural Networks (ANN)

## 📌 Project Overview

Fashion product classification is an important task in retail and e-commerce systems. Manually categorizing thousands of fashion products is time-consuming and error-prone.

This project develops an Artificial Neural Network (ANN) capable of automatically classifying clothing images into different fashion categories using the Fashion MNIST dataset.

The model learns visual patterns from grayscale clothing images and predicts the corresponding product category.

---

# 🎯 Problem Statement

Modern e-commerce platforms handle a massive number of clothing products daily. Manually assigning categories to these products can lead to inefficiencies and incorrect classifications.

This project aims to automate the fashion product categorization process by developing an Artificial Neural Network (ANN) that can classify clothing images into predefined fashion categories.

---

# 📂 Dataset Information

The project uses the Fashion MNIST dataset.

### Dataset Statistics

- Total Images: 70,000
- Training Images: 60,000
- Testing Images: 10,000
- Image Size: 28 × 28 Pixels
- Image Type: Grayscale
- Number of Classes: 10

### Classes

| Label | Category |
|---------|---------|
| 0 | T-Shirt/Top |
| 1 | Trouser |
| 2 | Pullover |
| 3 | Dress |
| 4 | Coat |
| 5 | Sandal |
| 6 | Shirt |
| 7 | Sneaker |
| 8 | Bag |
| 9 | Ankle Boot |

---

# 🛠 Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn

---

# 📊 Data Preprocessing

The following preprocessing steps were applied:

### 1. Normalization

Pixel values were converted from:

```text
0 - 255
```

to:

```text
0 - 1
```

This helps improve training stability and convergence.

### 2. Flattening

Each image was transformed from:

```text
28 × 28
```

to:

```text
784 Features
```

to make it compatible with the ANN architecture.

---

# 🧠 ANN Architecture

The developed ANN consists of:

```text
Input Layer (784 Features)
        ↓
Dense Layer (128 Neurons, ReLU)
        ↓
Batch Normalization
        ↓
Dropout (0.3)
        ↓
Dense Layer (64 Neurons, ReLU)
        ↓
Batch Normalization
        ↓
Dropout (0.3)
        ↓
Output Layer (10 Neurons, Softmax)
```

---

# ⚙️ Training Configuration

### Optimizer

```text
Adam Optimizer
```

### Loss Function

```text
Sparse Categorical Crossentropy
```

### Evaluation Metric

```text
Accuracy
```

### Epochs

```text
20
```

### Batch Size

```text
32
```

---

# 📈 Model Performance

### Training Accuracy

```text
86.73%
```

### Validation Accuracy

```text
87.57%
```

### Test Accuracy

```text
86.51%
```

### Test Loss

```text
0.3691
```

---

# 📉 Learning Curves

The model demonstrated:

✅ Increasing Training Accuracy

✅ Increasing Validation Accuracy

✅ Decreasing Training Loss

✅ Decreasing Validation Loss

These trends indicate that the model learned effectively without significant overfitting.

---

# 🔍 Confusion Matrix Analysis

The confusion matrix revealed that the model performed extremely well on visually distinct categories such as:

- Bag
- Sneaker
- Ankle Boot
- Trouser
- Sandal

However, the model occasionally confused visually similar classes such as:

- Shirt and T-Shirt
- Coat and Pullover
- Shirt and Coat

This behavior is expected because these categories share similar visual characteristics in low-resolution grayscale images.

---

# ✅ Results

The developed ANN achieved strong classification performance on the Fashion MNIST dataset.

Key achievements:

- Successfully classified 10 fashion categories.
- Achieved approximately 86.5% test accuracy.
- Demonstrated good generalization on unseen data.
- Reduced overfitting using Batch Normalization and Dropout.

---

# 📚 Concepts Applied

This project incorporates the following Deep Learning concepts:

### ANN Fundamentals

- Artificial Neural Networks
- Dense Layers
- ReLU Activation
- Softmax Activation

### Optimization Techniques

- Adam Optimizer

### Regularization Techniques

- Dropout
- Batch Normalization

### Model Evaluation

- Accuracy
- Loss Curves
- Confusion Matrix

---

# 🚀 Future Improvements

Potential enhancements include:

- Implementing Convolutional Neural Networks (CNNs)
- Applying Data Augmentation
- Hyperparameter Tuning
- Increasing Model Complexity
- Deploying the model using Streamlit or Flask

---

# 🎓 Learning Outcomes

Through this project, the following concepts were practiced:

- Dataset Exploration
- Data Preprocessing
- ANN Design
- Model Training
- Model Evaluation
- Prediction Analysis
- Confusion Matrix Interpretation
- Deep Learning Project Workflow

---

# 🏆 Conclusion

This project demonstrates how Artificial Neural Networks can be used to automate fashion product classification. Using the Fashion MNIST dataset, the developed model successfully learned meaningful visual patterns and achieved an impressive classification accuracy of 86.51% on unseen test data.

The project serves as a strong foundation for more advanced image classification tasks and future Computer Vision projects using Convolutional Neural Networks (CNNs).
