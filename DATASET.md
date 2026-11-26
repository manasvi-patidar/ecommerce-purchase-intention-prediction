# 📊 Dataset Documentation

This document provides an overview of the dataset used in **ShopSense AI – E-Commerce Purchase Intention Prediction**, including its characteristics, features, and target variable.

---

## 1. Dataset Overview

The dataset contains information about visitors browsing an e-commerce website. It captures their browsing behaviour, website interactions, session duration, traffic sources, and other characteristics.

The dataset is used to understand visitor behaviour and predict whether a visitor is likely to complete a purchase.

| Attribute          | Description                |
| ------------------ | -------------------------- |
| Dataset Domain     | E-Commerce                 |
| Total Records      | 12,330                     |
| Number of Features | 17                         |
| Data Type          | Numerical and Categorical  |
| Observation        | Individual visitor session |
| Target Variable    | `Revenue`                  |
| Problem Type       | Binary Classification      |
| Learning Type      | Supervised Learning        |

---

## 2. Dataset Context

An e-commerce company wants to better understand the behaviour of visitors browsing its online store.

Thousands of visitors interact with product pages and other website sections every day, but not all of them complete a purchase.

The company aims to identify visitors who are more likely to make a purchase based on their browsing behaviour and website session activities.

The dataset contains 12,330 individual visitor sessions collected over a period of one year. Each session represents a unique visitor, helping avoid the influence of repeated visits from the same users.

---

## 3. Feature Description

The dataset contains 17 features that capture different aspects of visitor behaviour and website interactions.

### Complete Feature Description

| Feature Name              | Description                                                                             |
| ------------------------- | --------------------------------------------------------------------------------------- |
| `Administrative`          | Number of pages visited related to account management, such as login and profile pages. |
| `Administrative_Duration` | Total time (in seconds) spent on administrative pages.                                  |
| `Informational`           | Number of informational pages visited, such as FAQs and policies.                       |
| `Informational_Duration`  | Total time (in seconds) spent on informational pages.                                   |
| `ProductRelated`          | Number of product-related pages visited.                                                |
| `ProductRelated_Duration` | Total time (in seconds) spent on product-related pages.                                 |
| `BounceRates`             | Percentage of visitors who leave the website after viewing one page.                    |
| `ExitRates`               | Percentage of exits from a page.                                                        |
| `PageValues`              | Average value of pages visited before completing a transaction.                         |
| `SpecialDay`              | Closeness of the visit date to a special day, such as Valentine's Day or Mother's Day.  |
| `Month`                   | Month in which the visit occurred (Feb, Mar, May, etc.).                                |
| `OperatingSystems`        | Operating system used by the visitor (encoded).                                         |
| `Browser`                 | Browser used by the visitor (encoded).                                                  |
| `Region`                  | Geographic region of the visitor (encoded).                                             |
| `TrafficType`             | Source of website traffic, such as direct visits, referrals, or advertisements.         |
| `VisitorType`             | Type of visitor: `Returning_Visitor`, `New_Visitor`, or `Other`.                        |
| `Weekend`                 | Indicates whether the visit occurred on a weekend.                                      |
| `Revenue`                 | Target variable indicating whether the visitor made a purchase.                         |

---

## 4. Target Variable

The target variable for this classification problem is:

**`Revenue`**

It indicates whether a visitor completed a purchase during their website session.

| Value   | Meaning                              |
| ------- | ------------------------------------ |
| `True`  | Visitor completed a purchase.        |
| `False` | Visitor did not complete a purchase. |

The objective is to predict the target variable using the visitor's session-related features.

---

## 5. Machine Learning Problem

Based on the dataset characteristics, this problem is formulated as:

- **Learning Type:** Supervised Learning
- **Problem Type:** Binary Classification
- **Algorithm:** Decision Tree Classifier
- **Target Variable:** `Revenue`

Since the dataset is imbalanced, the F1-score is selected as the primary evaluation metric.

The project uses an F1-score benchmark of **0.55** to assess model performance.

---

## 6. Dataset Characteristics

The dataset contains a combination of numerical and categorical features.

| Feature Category      | Examples                                                                       |
| --------------------- | ------------------------------------------------------------------------------ |
| Browsing Activity     | `Administrative`, `Informational`, `ProductRelated`                            |
| Session Duration      | `Administrative_Duration`, `Informational_Duration`, `ProductRelated_Duration` |
| Engagement Metrics    | `BounceRates`, `ExitRates`, `PageValues`                                       |
| Visit Information     | `Month`, `SpecialDay`, `Weekend`                                               |
| Visitor Information   | `VisitorType`, `Region`                                                        |
| Technical Information | `OperatingSystems`, `Browser`                                                  |
| Traffic Information   | `TrafficType`                                                                  |
| Target                | `Revenue`                                                                      |

---

## 7. Dataset Usage

The dataset is used throughout the project for:

1. Exploratory Data Analysis (EDA).
2. Understanding visitor browsing patterns.
3. Identifying relationships between features and purchase behaviour.
4. Data preprocessing and feature transformations.
5. Building a Decision Tree Classification model.
6. Applying pruning techniques to improve model performance.
7. Evaluating predictions using the F1-score.

---
