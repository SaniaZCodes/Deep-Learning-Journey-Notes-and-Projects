# 🚀 Advanced Optimizers

## Introduction

Advanced Optimizers improve the training process of neural networks by automatically adjusting learning rates during optimization.

In this section, we study:

- AdaGrad
- RMSProp
- Adam

These optimizers solve the limitations of traditional Gradient Descent and help neural networks converge faster and more efficiently.

---

# 1. AdaGrad (Adaptive Gradient)

## Concept

AdaGrad adapts the learning rate for each parameter individually.

- Frequently updated parameters receive smaller learning rates.
- Rarely updated parameters receive larger learning rates.

This makes AdaGrad particularly useful for sparse datasets.

## Advantages

✅ Adaptive learning rates

✅ Works well with sparse data

✅ Useful in NLP tasks

## Disadvantages

❌ Learning rate continuously decreases

❌ Training may stop too early

## TensorFlow Implementation

```python
import tensorflow as tf

optimizer = tf.keras.optimizers.Adagrad(
    learning_rate=0.01
)

model.compile(
    optimizer=optimizer,
    loss='categorical_crossentropy',
    metrics=['accuracy']
)
```

---

# 2. RMSProp (Root Mean Square Propagation)

## Concept

RMSProp was introduced to solve AdaGrad's learning-rate decay problem.

Instead of storing all previous gradients, RMSProp only focuses on recent gradients.

This prevents the learning rate from becoming extremely small.

## Advantages

✅ Solves AdaGrad's major limitation

✅ Faster convergence

✅ Stable training

✅ Effective for deep neural networks

## Disadvantages

❌ Requires hyperparameter tuning

❌ Can sometimes be outperformed by Adam

## TensorFlow Implementation

```python
import tensorflow as tf

optimizer = tf.keras.optimizers.RMSprop(
    learning_rate=0.001
)

model.compile(
    optimizer=optimizer,
    loss='categorical_crossentropy',
    metrics=['accuracy']
)
```

---

# 3. Adam (Adaptive Moment Estimation)

## Concept

Adam combines the strengths of:

- Momentum
- RMSProp

It adapts learning rates while also using information from previous gradients.

Adam is currently the most widely used optimizer in Deep Learning.

## Advantages

✅ Fast convergence

✅ Adaptive learning rates

✅ Stable training

✅ Less hyperparameter tuning

✅ Works well on most deep learning tasks

## Disadvantages

❌ Slightly higher memory usage

❌ SGD may sometimes generalize better

## TensorFlow Implementation

```python
import tensorflow as tf

optimizer = tf.keras.optimizers.Adam(
    learning_rate=0.001
)

model.compile(
    optimizer=optimizer,
    loss='categorical_crossentropy',
    metrics=['accuracy']
)
```

---

# Comparison

| Optimizer | Main Idea | Major Strength | Major Weakness |
|------------|------------|------------|------------|
| AdaGrad | Adaptive Learning Rate | Works well with sparse data | Learning rate becomes very small |
| RMSProp | Uses Recent Gradients | Prevents learning-rate decay | Requires tuning |
| Adam | Momentum + RMSProp | Fast and stable training | Higher memory usage |

---

# Key Takeaways

- AdaGrad introduced adaptive learning rates.
- RMSProp solved AdaGrad's learning-rate decay problem.
- Adam combines Momentum and RMSProp.
- Adam is the most commonly used optimizer in modern Deep Learning.
- Advanced Optimizers improve convergence speed and training stability.

---

# Conclusion

AdaGrad, RMSProp, and Adam are advanced optimization algorithms that improve neural network training by adapting learning rates during optimization. Among them, Adam is the most popular because it combines the benefits of both Momentum and RMSProp, resulting in faster and more stable convergence.
