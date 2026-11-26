
# 🛍️ ShopSense AI

### E-Commerce Purchase Intention Prediction

**Turning browsing behaviour into buying insights.**

ShopSense AI is an end-to-end supervised machine learning project that predicts whether an e-commerce visitor is likely to make a purchase based on their browsing behaviour and website session activities.

The project focuses on analyzing customer interactions, identifying purchasing patterns, and building an optimized Decision Tree Classification model to predict purchase intentions.

---

## 🎯 Problem Statement

E-commerce platforms receive thousands of visitors every day, but only a fraction of them complete a purchase.

Understanding which visitors are likely to make a purchase can help businesses improve their marketing strategies, optimize customer engagement, and identify potential buyers.

ShopSense AI aims to solve this problem by analyzing visitor session data and predicting whether a browsing session will result in a purchase.

---

## 📊 Dataset Overview

The project uses an e-commerce visitor session dataset containing **12,330 records** collected over a period of one year.

Each record represents a unique visitor session and contains numerical and categorical features describing browsing behaviour.

### Key Features

| Feature | Description |
|---|---|
| Administrative | Number of administrative pages visited |
| Administrative_Duration | Time spent on administrative pages |
| Informational | Number of informational pages visited |
| Informational_Duration | Time spent on informational pages |
| ProductRelated | Number of product-related pages visited |
| ProductRelated_Duration | Time spent on product-related pages |
| BounceRates | Percentage of visitors leaving after viewing one page |
| ExitRates | Percentage of exits from a page |
| PageValues | Average value of pages visited before a transaction |
| SpecialDay | Closeness of the visit date to a special day |
| Month | Month of the visit |
| OperatingSystems | Operating system used by the visitor |
| Browser | Browser used by the visitor |
| Region | Geographic region of the visitor |
| TrafficType | Source of website traffic |
| VisitorType | Type of visitor |
| Weekend | Whether the visit occurred on a weekend |

**Target Variable:** `Revenue`

- `True` – Visitor completed a purchase.
- `False` – Visitor did not complete a purchase.

### 📚 Documentation

- [Dataset Information](DATASET.md)

---

## ⚙️ Project Workflow

1. Exploratory Data Analysis (EDA)
2. Data Cleaning and Preprocessing
3. Feature Engineering
4. Handling Class Imbalance
5. Decision Tree Classification
6. Hyperparameter Tuning
7. Decision Tree Pruning
   - Pre-Pruning
   - Post-Pruning
8. Model Evaluation and Comparison

---

## 🤖 Machine Learning Approach

**Algorithm:** Decision Tree Classifier

**Optimization Techniques:**

- Pre-Pruning
- Post-Pruning using Cost Complexity Pruning
- Hyperparameter Tuning

Pruning techniques are explored to control tree complexity, reduce overfitting, and improve model generalization.

---

## 📈 Model Evaluation

Since the dataset is imbalanced, the **F1-score** is used as the primary evaluation metric.

**Target F1-score: 0.55 or above**

Additional evaluation metrics:

- Accuracy
- Precision
- Recall
- Confusion Matrix

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
