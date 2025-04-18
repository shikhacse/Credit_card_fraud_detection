# 💳 Credit Card Fraud Detection — EDA + Machine Learning

This project analyzes real-world credit card transaction data to detect fraudulent activities. It tackles the challenge of extreme data imbalance and builds robust machine learning models.

---

## 📚 Table of Contents
- [1. Project Overview](#1-project-overview)
- [2. Dataset Information](#2-dataset-information)
- [3. Exploratory Data Analysis (EDA)](#3-exploratory-data-analysis-eda)
- [4. Data Preprocessing](#4-data-preprocessing)
- [5. Model Building and Evaluation](#5-model-building-and-evaluation)
- [6. Conclusion](#6-conclusion)

---

## 1. Project Overview
- **Problem:** Credit card frauds cause massive financial losses globally.
- **Goal:** Predict whether a transaction is fraudulent (1) or genuine (0).
- **Challenge:** Highly imbalanced data — very few fraud cases.
- **Solution:** 
  - Perform detailed EDA.
  - Handle imbalance using **SMOTE + Undersampling**.
  - Build and compare machine learning models.

---

## 2. Dataset Information
- **Features:**
  - `V1` to `V28`: Transformed using PCA for confidentiality.
  - `Time`: Seconds elapsed since first transaction.
  - `Amount`: Transaction amount.
  - `Class`: Target variable (0 = No Fraud, 1 = Fraud).
- **Rows:** ~284,807  
- **Size:** ~67 MB

---

## 3. Exploratory Data Analysis (EDA)
- ✅ Checked for missing values (no missing data).
- ✅ Visualized class imbalance (Fraud vs No Fraud).
- ✅ Observed feature distributions for fraud vs non-fraud cases.

**Key Insights:**
- Fraudulent transactions have different patterns in `V1`, `V2`, `V3`, etc.
- The `Amount` for frauds tends to vary differently compared to normal transactions.

---

## 4. Data Preprocessing
- **Feature Selection:**
  - Selected important features using correlation matrix and ANOVA scores.
- **Data Balancing:**
  - Applied **Random Undersampling** and **SMOTE** to fix imbalance.
- **Train-Test Split:**
  - 80% training, 20% testing.

---

## 5. Model Building and Evaluation
**Models Trained:**
- Logistic Regression
- Support Vector Classifier (SVC)
- Decision Tree Classifier
- Random Forest Classifier
- K-Nearest Neighbors (KNN)

**Evaluation Metrics:**
- Cross-validation scores
- ROC-AUC scores
- Confusion matrices
- Classification reports (Precision, Recall, F1-score)

**Key Observations:**
- KNN performed the best with the highest ROC-AUC.
- Logistic Regression and Random Forest also performed well.

---

## 6. Conclusion
✅ Successfully built multiple ML models to detect credit card fraud.

✅ Addressed data imbalance effectively using SMOTE + Undersampling.

✅ KNN achieved the best performance, closely followed by Logistic Regression and Random Forest.

✅ Highlighted the importance of proper preprocessing when working with imbalanced datasets.

---

# 📂 Project Structure

| File | Description |
|:---|:---|
| `credit_card_fraud_detection.ipynb` | Complete notebook (EDA + Preprocessing + ML Models) |
| `creditcard.csv` | Raw dataset |
| `README.md` | Project Overview (this file) |

---
