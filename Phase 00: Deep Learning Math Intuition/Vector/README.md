# 🧮 Deep Learning Math Intuition

## 📌 Topic 01: What is a Vector?

Before learning Neural Networks, it is important to understand the basic mathematical building blocks used in Deep Learning.

One of the most important building blocks is:

# 🎯 Vector

A vector is simply an **ordered collection of numbers**.

In Machine Learning and Deep Learning, vectors are used to represent data points.

---

# 🤔 Why Do We Need Vectors?

Computers and Neural Networks do not understand concepts like:

```text
Age

Income

CGPA

Projects
```

Instead, they see everything as numbers.

For example:

```text
Age = 22

CGPA = 3.5

Projects = 4
```

can be represented as:

```text
[22, 3.5, 4]
```

This representation is called a **Vector**.

---

# 📚 Examples of Vectors

### Student Information

```text
[22, 3.5, 4]
```

Meaning:

```text
Age = 22

CGPA = 3.5

Projects = 4
```

---

### Customer Information

```text
[25, 50000, 120]
```

Meaning:

```text
Age = 25

Income = 50000

Spending Score = 120
```

---

### Fraud Detection Example

```text
[100, 2, 5, 200]
```

Meaning:

```text
Time = 100

V1 = 2

V2 = 5

Amount = 200
```

---

# 🧠 Vector in Machine Learning

Every row of a dataset can be represented as a vector.

Example:

| Age | Income | Spending Score |
|------|--------|---------------|
| 25 | 50000 | 120 |

can be represented as:

```text
[25, 50000, 120]
```

---

# 🚀 Vector in Deep Learning

Neural Networks work with vectors.

Whenever we provide input to a Neural Network:

```text
Data
    ↓
Vector
    ↓
Neural Network
```

The Neural Network processes vectors and learns patterns from them.

---

# 🎯 Real-World Intuition

Think of a vector as a summary of an object.

### Student

```text
[Age, CGPA, Projects]
```

---

### Customer

```text
[Age, Income, Spending]
```

---

### Transaction

```text
[Time, V1, V2, Amount]
```

Each vector completely represents one observation.

---

# ✅ Key Points

- A vector is an ordered collection of numbers.
- Every data point can be represented as a vector.
- Neural Networks use vectors as inputs.
- Machine Learning models work with vectors internally.
- A vector usually represents a single observation or record.

---

# 🎓 Interview Question

### What is a Vector?

A vector is an ordered collection of numbers used to represent a single observation or data point in Machine Learning and Deep Learning.

---

# 🌟 Memory Trick

```text
One Observation
        ↓
Vector
```

Examples:

```text
Student
        ↓
[Age, CGPA, Projects]

Transaction
        ↓
[Time, V1, V2, Amount]
```

---

# 🏁 Conclusion

A Vector is one of the most fundamental concepts in Deep Learning. Every input provided to a Neural Network is ultimately converted into vectors. Understanding vectors makes it easier to later understand matrices, Neural Networks, and Deep Learning architectures.
