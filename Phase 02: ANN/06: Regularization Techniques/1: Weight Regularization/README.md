# 🛡️ Weight Regularization

## Introduction

Overfitting occurs when a neural network performs exceptionally well on training data but fails to generalize to unseen data.

One of the major causes of overfitting is large weight values. Weight Regularization helps control these weights by adding a penalty term to the loss function during training.

In this section, we study:

- L1 Regularization
- L2 Regularization

Both techniques reduce overfitting but use different approaches to penalize large weights.

---

# 1. L1 Regularization

## Concept

L1 Regularization adds the sum of the absolute values of all weights to the loss function.

### Formula

L1 Penalty = |w₁| + |w₂| + |w₃| + ... + |wₙ|

### Modified Loss Function

Loss = Original Loss + λ(|w₁| + |w₂| + ... + |wₙ|)

Where:

- λ (Lambda) controls the strength of regularization.
- Larger λ means stronger regularization.

---

## How L1 Works

L1 pushes less important weights toward zero.

As training progresses:

- Important features keep non-zero weights.
- Unimportant features receive weights close to or equal to zero.

This makes L1 useful for automatic feature selection.

---

## Advantages

✅ Reduces overfitting

✅ Performs feature selection

✅ Produces sparse models

✅ Removes unimportant features automatically

---

## Disadvantages

❌ Can remove too many features

❌ Less stable than L2 in some situations

---

## TensorFlow Implementation

```python
from tensorflow.keras import regularizers
from tensorflow.keras.models import Sequential
from tensorflow.keras.layers import Dense

model = Sequential([
    Dense(
        128,
        activation='relu',
        kernel_regularizer=regularizers.l1(0.001)
    ),
    Dense(1, activation='sigmoid')
])
```

---

# 2. L2 Regularization

## Concept

L2 Regularization adds the sum of squared weight values to the loss function.

Instead of forcing weights to become zero, it reduces their magnitude.

### Formula

L2 Penalty = w₁² + w₂² + w₃² + ... + wₙ²

### Modified Loss Function

Loss = Original Loss + λ(w₁² + w₂² + ... + wₙ²)

Where:

- λ (Lambda) controls regularization strength.
- Larger λ results in stronger weight shrinking.

---

## How L2 Works

L2 discourages large weights by shrinking them during training.

As training progresses:

- Large weights become smaller.
- Important features remain in the model.
- Overfitting is reduced.

Unlike L1, weights usually do not become exactly zero.

---

## Advantages

✅ Reduces overfitting

✅ Stable training

✅ Keeps all features

✅ Most commonly used regularization technique

✅ Works well in Deep Learning applications

---

## Disadvantages

❌ Does not perform feature selection

❌ Unimportant features usually remain in the model

---

## TensorFlow Implementation

```python
from tensorflow.keras import regularizers
from tensorflow.keras.models import Sequential
from tensorflow.keras.layers import Dense

model = Sequential([
    Dense(
        128,
        activation='relu',
        kernel_regularizer=regularizers.l2(0.001)
    ),
    Dense(1, activation='sigmoid')
])
```

---

# L1 vs L2 Regularization

| Feature | L1 Regularization | L2 Regularization |
|----------|----------|----------|
| Penalty Type | Absolute Values | Squared Values |
| Formula | \|w\| | w² |
| Feature Selection | Yes | No |
| Produces Zero Weights | Yes | Usually No |
| Model Type | Sparse Model | Dense Model |
| Stability | Less Stable | More Stable |
| Deep Learning Usage | Less Common | More Common |

---

# Key Takeaways

- Regularization helps prevent overfitting.
- L1 uses absolute values of weights as a penalty.
- L2 uses squared values of weights as a penalty.
- L1 can force weights to become exactly zero and perform feature selection.
- L2 shrinks weights while keeping most features in the model.
- L2 Regularization is more commonly used in Deep Learning.

---

# Conclusion

Weight Regularization is a powerful technique for reducing overfitting in neural networks. L1 Regularization performs feature selection by forcing some weights to become zero, while L2 Regularization reduces overfitting by shrinking large weights. Among the two, L2 is the most commonly used regularization method in modern Deep Learning applications.
