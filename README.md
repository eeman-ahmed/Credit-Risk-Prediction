# Credit-Risk-Prediction

## Overview
This project predicts whether a loan applicant is likely to default on a loan using the Kaggle Loan Prediction Dataset (https://www.kaggle.com/datasets/devzohaib/eligibility-prediction-for-loan).

I practiced:
- Data cleaning (handling missing values: median for numeric, mode for categorical)
- Encoding categorical variables
- Exploratory Data Analysis (EDA)
- Building classification models: Logistic Regression and Decision Tree
- Evaluating models using Accuracy, Recall, Confusion Matrix, and ROC-AUC

## Dataset
- Source: Kaggle (Loan Prediction Dataset)
- Features: Applicant Income, Loan Amount, Education, Property Area, Credit History, etc.
- Target: Loan_Status (0 = Default, 1 = Non-default)

## Results
| Model               | Accuracy | Recall (Class 0) | AUC   |
|----------------------|----------|------------------|-------|
| Logistic Regression  | 0.86     | 0.58             | 0.85  |
| Decision Tree        | 0.84     | 0.54             | 0.77  |

- Logistic Regression performed better overall (higher AUC and balanced performance).
- Both models correctly identified most approvals but struggled with rejections (Class 0).

## Visuals
*ROC Curve Comparison for Logistic Regression and Decision Tree.*

## How to Run
```bash
pip install -r requirements.txt
jupyter notebook LoanPrediction.ipynb
