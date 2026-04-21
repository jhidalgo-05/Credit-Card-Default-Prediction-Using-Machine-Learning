# CreditRiskIQ: Credit Card Default Prediction

## 📊 Overview
CreditRiskIQ is a machine learning project focused on predicting whether a credit card client will default on their next payment. Using the UCI Credit Card Default dataset, this project explores financial behavior, payment history, and demographic factors to build predictive models for credit risk assessment.

This project demonstrates an end-to-end data science workflow including data cleaning, exploratory data analysis (EDA), feature engineering, and classification modeling.

---

## 🎯 Objective
The goal of this project is to:
- Predict credit card default risk (`default.payment.next.month`)
- Identify key features influencing default behavior
- Build and compare machine learning models for classification

---

## 📁 Dataset
- Source: UCI Machine Learning Repository
- Dataset: Default of Credit Card Clients
- Features include:
  - Demographics: `SEX`, `EDUCATION`, `MARRIAGE`, `AGE`
  - Credit limit: `LIMIT_BAL`
  - Payment history: `PAY_1` to `PAY_6`
  - Bill amounts: `BILL_AMT1` to `BILL_AMT6`
  - Payment amounts: `PAY_AMT1` to `PAY_AMT6`

Target variable:
- `default.payment.next.month` (1 = default, 0 = no default)

---

## 🧹 Data Cleaning Steps
- Renamed inconsistent columns (e.g., `PAY_0` → `PAY_1`)
- Handled invalid categorical values in `EDUCATION` and `MARRIAGE`
- Treated undocumented values in payment history variables (e.g., `-2`)
- Checked and confirmed absence of missing values
- Removed duplicate records

---

## 📊 Exploratory Data Analysis (EDA)
Key insights explored:
- Default rate distribution (class imbalance)
- Correlation between repayment status and default
- Impact of credit limit on default risk

Visualizations used:
- Correlation heatmap
- Distribution plots
- Bar charts (categorical analysis)

---

## ⚙️ Feature Engineering
- Total bill amount across months
- Total payment amount
- Payment ratio (payments vs bills)
- Maximum delay across months
- Number of late payments

---

## 📈 Evaluation Metrics
Due to class imbalance, the following metrics were used:
- ROC-AUC Score
- Precision / Recall
- F1-Score
- Confusion Matrix

---

## 🧠 Key Insights
- Payment history variables are the strongest predictors of default
- Credit limit is negatively correlated with default risk
- Clients with frequent delays have significantly higher default probability
- Class imbalance must be handled carefully to avoid misleading accuracy

---

## 🛠️ Tech Stack
- Python
- Pandas & NumPy
- Matplotlib & Seaborn
- Scikit-learn
- Pytorch

---


## 📌 Collaborators
Joaquin Hidalgo  
Matheus Gomes
Natiana Urdaneta
Rajan Jinadra
---

## 📜 License
This project is for educational purposes.
