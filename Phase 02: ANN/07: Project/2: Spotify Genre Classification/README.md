# 🎵 Spotify Genre Classification Using Artificial Neural Networks (ANN)

## 📌 Project Overview

Music streaming platforms contain thousands of songs belonging to different genres. Manually organizing and categorizing songs can be difficult and time-consuming.

This project develops an Artificial Neural Network (ANN) that predicts the genre of a song using its audio characteristics such as danceability, energy, loudness, tempo, acousticness, and other Spotify audio features.

---

# 🎯 Problem Statement

The objective of this project is to build a multiclass classification system capable of predicting the genre of a song using Spotify audio features.

The model learns patterns from audio characteristics and classifies songs into one of 114 music genres.

---

# 🏪 Practical Application

Such systems can be useful in:

- Music recommendation systems
- Music library organization
- Automatic genre classification
- Playlist generation
- Music analytics

---

# 📂 Dataset Information

Dataset: Spotify Tracks Dataset

### Dataset Statistics

- Total Records: 114,000
- Total Features: 15
- Total Genres: 114
- Target Variable: `track_genre`

---

# 🔍 Exploratory Data Analysis (EDA)

The following EDA steps were performed:

- Missing Value Analysis
- Duplicate Value Analysis
- Distribution Analysis
- Skewness Analysis
- Correlation Analysis
- Outlier Detection

### Key Findings

- Only one record contained missing values and was removed.
- No duplicate records were found.
- Several features showed skewed distributions.
- Outliers were present but represented valid musical characteristics and were retained.
- No severe correlation was found between features.

---

# ⚙️ Data Preprocessing

The following preprocessing steps were applied:

### 1. Missing Value Handling

Rows containing missing values were removed.

### 2. Feature Selection

The following columns were removed because they were not directly useful for genre prediction:

- Unnamed: 0
- track_id
- track_name
- album_name
- artists

### 3. Train-Test Split

Dataset was divided into:

- 80% Training Data
- 20% Testing Data

### 4. Label Encoding

The target variable (`track_genre`) was converted into numerical labels.

### 5. Feature Scaling

StandardScaler was used to standardize the feature values before training the ANN.

---

# 🧠 ANN Architecture

## Experiment 1

```text
Input Layer (15 Features)
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
Output Layer (114 Neurons, Softmax)
```

---

## Experiment 2 (Final Model)

```text
Input Layer (15 Features)
        ↓
Dense Layer (256 Neurons, ReLU)
        ↓
Batch Normalization
        ↓
Dropout (0.2)
        ↓
Dense Layer (128 Neurons, ReLU)
        ↓
Batch Normalization
        ↓
Dropout (0.2)
        ↓
Dense Layer (64 Neurons, ReLU)
        ↓
Batch Normalization
        ↓
Output Layer (114 Neurons, Softmax)
```

---

# ⚙️ Training Configuration

### Optimizer

Adam Optimizer

### Loss Function

Sparse Categorical Crossentropy

### Regularization Techniques

- Batch Normalization
- Dropout
- Early Stopping

---

# 📊 Model Performance

## Experiment 1

- Test Accuracy: **30.44%**
- Test Loss: **2.6599**

---

## Experiment 2 (Final Model)

- Training Accuracy: **31.01%**
- Validation Accuracy: **32.69%**
- Test Accuracy: **32.65%**
- Test Loss: **2.4914**

---

# 🏆 Model Comparison

| Model | Test Accuracy | Test Loss |
|---------|---------|---------|
| Experiment 1 | 30.44% | 2.6599 |
| Experiment 2 | 32.65% | 2.4914 |

Experiment 2 achieved higher accuracy and lower loss and was selected as the final model.

---

# 📈 Training Analysis

The training and validation curves showed:

- Continuous improvement in accuracy
- Continuous reduction in loss
- Stable learning behavior
- No significant signs of overfitting

---

# 📚 Concepts Applied

### Deep Learning

- Artificial Neural Networks (ANN)
- Dense Layers
- ReLU Activation Function
- Softmax Activation Function

### Optimization

- Adam Optimizer

### Regularization

- Batch Normalization
- Dropout
- Early Stopping

### Data Preprocessing

- Missing Value Handling
- Feature Selection
- Label Encoding
- Feature Scaling

---

# 🎓 Learning Outcomes

Through this project, I gained hands-on experience in:

- Exploratory Data Analysis (EDA)
- Real-world data preprocessing
- Feature engineering and selection
- Building Artificial Neural Networks
- Hyperparameter experimentation
- Model evaluation and comparison
- Multiclass classification problems

---

# 🏁 Conclusion

This project demonstrates how Artificial Neural Networks can be applied to music genre classification using Spotify audio features.

After performing data preprocessing, exploratory data analysis, and multiple ANN experiments, the final model achieved a test accuracy of 32.65% across 114 different genres.

The project provided practical experience in developing, evaluating, and comparing ANN models on real-world tabular data.
