# Loan Approval Prediction

A machine learning project that predicts loan approval outcomes using classification models.  
Developed as part of the Data Science course (Fall 2024) at FAST-NUCES, Lahore.

---

## Overview

This project builds a classification system to predict whether a loan application will be approved based on applicant financial and risk-related features. The goal is to compare multiple models and identify the most effective approach.

---

## Dataset

- **Size:** 20,000 records  
- **Features:** 36 (numerical + categorical)  
- **Target:** `LoanApproved` (binary classification)

Key predictors include:
- Risk Score
- Annual Income
- Monthly Income
- Interest Rate
- Debt-to-Income Ratio

---

## Methodology

- Data cleaning and missing value handling  
- One-hot encoding for categorical variables  
- Outlier removal using IQR method  
- Feature scaling using Min-Max normalization  
- Feature selection using forward selection  
- Exploratory data analysis using correlation analysis  

---

## Models Evaluated

| Model | Features Used | Accuracy |
|------|---------------|----------|
| Logistic Regression | Multiple financial features | 97.75% |
| Random Forest | RiskScore | **99.19%** |
| KNN (k=3) | RiskScore, AnnualIncome | 98.15% |

---

## Key Result

- **Random Forest performed best with 99.19% accuracy**
- `RiskScore` emerged as the strongest predictive feature
- Simpler feature sets performed competitively, especially with tree-based models

---

## Tech Stack

- Python  
- Jupyter Notebook  
- scikit-learn  
- pandas, NumPy  
- Matplotlib, Seaborn  

---

## Project Structure

```
NLP-project/
│
├── Notebook/
│   └── Loan_Approval_Prediction.ipynb
│
├── Report/
│   └── Project-report.pdf
│
└── README.md
```

---

## Summary

This project demonstrates that:
- Tree-based models outperform linear models for this dataset
- Strong predictive signals exist in a few key financial features
- Proper preprocessing significantly improves classification performance

---
