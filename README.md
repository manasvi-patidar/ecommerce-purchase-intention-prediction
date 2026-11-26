# 🛍️ ShopSense AI

### E-Commerce Purchase Intention Prediction

**Turning browsing behaviour into buying insights.**

ShopSense AI is a supervised machine learning project that predicts whether an e-commerce visitor is likely to make a purchase based on their browsing behaviour and website session activities.

The project uses a Decision Tree Classification model to analyze visitor interactions and identify purchasing patterns.

---

## 🎯 Problem Statement

E-commerce websites receive thousands of visitors every day, but only a fraction of them complete a purchase.

Understanding visitor purchase intentions can help businesses improve marketing strategies, optimize customer engagement, and identify potential buyers.

ShopSense AI aims to predict whether a browsing session will result in a purchase by analyzing visitor session data.

---

## 📊 Dataset Overview

The project uses the **Online Shoppers Purchasing Intention Dataset**, containing 12,330 visitor sessions collected over a one-year period.

| Attribute       | Description                        |
| --------------- | ---------------------------------- |
| Total Records   | 12,330                             |
| Input Features  | 17                                 |
| Target Variable | `Revenue`                          |
| Problem Type    | Binary Classification              |
| Learning Type   | Supervised Learning                |
| Data Types      | Numerical, Categorical and Boolean |

### Target Variable

`Revenue` represents whether a visitor completed a purchase.

- `True` – Visitor completed a purchase.
- `False` – Visitor did not complete a purchase.

The dataset contains an imbalanced target distribution, making F1-score an important evaluation metric.

### 📚 Documentation

- [Dataset Information](DATASET.md)

---

## ⚙️ Project Workflow

1. Dataset Loading
2. Feature and Target Separation
3. Train-Test Splitting
4. Numerical and Categorical Feature Preprocessing
5. Decision Tree Classification
6. Model Training and Evaluation
7. Hyperparameter Tuning using GridSearchCV
8. Best Model Evaluation

---

## 🤖 Machine Learning Approach

**Algorithm:** Decision Tree Classifier

### Data Preprocessing

A Scikit-learn preprocessing pipeline is used to handle different feature types.

- **StandardScaler:** Scales numerical features.
- **OneHotEncoder:** Encodes categorical features.
- **ColumnTransformer:** Applies appropriate transformations to different feature groups.
- **Pipeline:** Combines preprocessing and model training into a single workflow.

### Model Configuration

The Decision Tree Classifier uses:

- `max_depth=6`
- `min_samples_leaf=30`
- `class_weight="balanced"`
- `random_state=42`

Class weighting is used to address the imbalanced target distribution.

### Hyperparameter Tuning

GridSearchCV with 5-fold cross-validation is used to identify suitable Decision Tree hyperparameters.

Parameters explored:

- `max_depth`: [4, 6, 8]
- `min_samples_leaf`: [20, 30, 50]

The F1-score is used as the model selection metric.

---

## 📈 Model Evaluation

Since the dataset contains an imbalanced target variable, **F1-score** is used as the primary evaluation metric.

The model is evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix
- Classification Report

---

## 📁 Project Structure

```text
ShopSense AI/
│
├── dataset/
│   └── shop_sense_ecommerce.csv
│
├── notebook/
│   └── shop_sense.ipynb
│
├── .gitignore
├── DATASET.md
├── README.md
└── requirements.txt
```

---

## 🛠️ Tech Stack

- Python
- NumPy, Pandas
- Matplotlib, Seaborn
- Scikit-learn
- Jupyter Notebook, VS Code
- Git, GitHub

---

## 👩‍💻 Author

**Manasvi Patidar**

[GitHub](https://github.com/manasvi-patidar)

---
