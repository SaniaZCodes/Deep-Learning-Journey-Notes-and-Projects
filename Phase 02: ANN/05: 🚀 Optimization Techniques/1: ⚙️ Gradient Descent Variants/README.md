# ⚙️ Gradient Descent Variants

## 📌 Overview

Gradient Descent is one of the most important optimization techniques in Deep Learning.

Its purpose is to reduce the loss function by updating the weights of a Neural Network and improving predictions over time.

Different variants of Gradient Descent were developed to improve training speed, efficiency, and stability.

This category covers:

- Batch Gradient Descent
- Stochastic Gradient Descent (SGD)
- Mini Batch Gradient Descent

---

# 🎯 Why Do We Need Gradient Descent?

After:

```text
Prediction
      ↓

Loss Function
      ↓

Error
      ↓

Backpropagation
```

the Neural Network knows where the mistake occurred.

Gradient Descent helps update the weights so that future predictions become better.

---

# 🚀 Batch Gradient Descent

## What is Batch Gradient Descent?

Batch Gradient Descent updates the weights only after processing the entire training dataset.

### Workflow

```text
Entire Dataset
       ↓

Calculate Error
       ↓

Update Weights Once
```

### Example

Dataset:

```text
60,000 Images
```

The model processes all:

```text
60,000 Images
```

before making a single weight update.

---

## ✅ Advantages

- Stable learning
- Accurate gradient calculation
- Smooth weight updates

---

## ❌ Disadvantages

- Slow for large datasets
- High computational cost
- Requires more memory

---

# 🚀 Stochastic Gradient Descent (SGD)

## What is SGD?

Stochastic Gradient Descent updates weights after processing each training sample individually.

### Workflow

```text
One Sample
      ↓

Calculate Error
      ↓

Update Weights
```

This process repeats for every sample.

---

## Example

```text
Image 1
   ↓
Update

Image 2
   ↓
Update

Image 3
   ↓
Update
```

---

## ✅ Advantages

- Faster learning
- Immediate feedback
- Useful for very large datasets

---

## ❌ Disadvantages

- Noisy updates
- Less stable learning
- Training fluctuations

---

# 🚀 Mini Batch Gradient Descent

## What is Mini Batch Gradient Descent?

Mini Batch Gradient Descent updates weights after processing a small subset of training samples called a batch.

It combines the benefits of Batch Gradient Descent and SGD.

### Workflow

```text
Small Batch
      ↓

Calculate Error
      ↓

Update Weights
```

---

## Example

Dataset:

```text
60,000 Images
```

Batch Size:

```text
32
```

Process:

```text
32 Images
      ↓
Update

Next 32 Images
      ↓
Update

Next 32 Images
      ↓
Update
```

---

## ✅ Advantages

- Faster than Batch Gradient Descent
- More stable than SGD
- Efficient memory usage
- Most commonly used in Deep Learning

---

## ❌ Disadvantages

- Requires selecting a suitable batch size
- Very small batches behave like SGD
- Very large batches behave like Batch Gradient Descent

---

# 📊 Comparison

| Technique | Data Used Before Weight Update |
|------------|-------------------------------|
| Batch Gradient Descent | Entire Dataset |
| SGD | One Training Sample |
| Mini Batch Gradient Descent | Small Batch of Samples |

---

# 🎯 Which Variant is Most Commonly Used?

In modern Deep Learning:

✅ Mini Batch Gradient Descent

because it provides:

```text
Good Speed
      +
Good Stability
```

---

# ✅ Key Points

### Batch Gradient Descent

- Uses entire dataset
- Stable but slow

### SGD

- Uses one sample
- Fast but noisy

### Mini Batch Gradient Descent

- Uses small batches
- Fast and stable
- Most practical approach

---

# 🎓 Interview Questions

### What is Batch Gradient Descent?

Batch Gradient Descent updates weights after processing the entire training dataset.

---

### What is Stochastic Gradient Descent?

SGD updates weights after processing each individual training sample.

---

### What is Mini Batch Gradient Descent?

Mini Batch Gradient Descent updates weights after processing a small subset of samples called a batch.

---

### Which Gradient Descent variant is most commonly used?

Mini Batch Gradient Descent.

---

# 🌟 Memory Trick

```text
Batch GD
      ↓
Whole Dataset
```

```text
SGD
      ↓
One Sample
```

```text
Mini Batch GD
      ↓
Small Group Of Samples
```

---

# 🏁 Conclusion

Batch Gradient Descent, Stochastic Gradient Descent, and Mini Batch Gradient Descent are different strategies for updating Neural Network weights. Among them, Mini Batch Gradient Descent is the most widely used because it provides a practical balance between training speed and learning stability.
