# Credit Card Fraud Detection using Cost-Sensitive Learning

## Overview
This project builds machine learning models to detect fraudulent credit card transactions from a highly imbalanced dataset (284,807 transactions with 0.17% fraud cases).

The focus is on handling class imbalance using cost-sensitive learning and evaluating models using appropriate metrics such as ROC-AUC and PR-AUC.

---

## Dataset
- Source: Kaggle Credit Card Fraud Detection Dataset
- Data Set Link:" https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud "
- Total Transactions: 284,807
- Fraud Cases: 492 (0.172%)

---

## Problem
Traditional accuracy metrics are misleading for imbalanced datasets.  
Goal: Maximize fraud detection (Recall) while maintaining high Precision.

---

## Techniques Used

- Stratified Train-Test Split
- Class-weight balancing
- Feature scaling
- Imbalance-aware modeling

---

## Models Implemented

- Logistic Regression
- Random Forest
- XGBoost

---

## Evaluation Metrics

- Precision
- Recall
- F1-score
- ROC-AUC
- PR-AUC

---

## Results

| Model | Precision | Recall | F1 | ROC-AUC |
|--------|-----------|--------|----|---------|
| Logistic Regression | 0.92 | 0.60 | 0.73 | 0.96 |
| Random Forest | 0.95 | 0.84 | 0.89 | 0.98 |
| XGBoost | 0.97 | 0.85 | 0.90 | 0.99 |

XGBoost achieved the best balance between precision and recall.

---

## Key Learnings

- Accuracy is not suitable for imbalanced datasets.
- PR-AUC is more informative than ROC-AUC in extreme imbalance.
- Class-weighting improves minority class detection.
- Ensemble methods outperform linear models for fraud detection.

---

## Future Improvements

- SMOTE oversampling comparison
- Hyperparameter tuning with GridSearchCV
- Model deployment using Streamlit
