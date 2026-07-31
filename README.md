# UC Berkeley Professional Certificate in Machine Learning & AI
## Module 20 – Credit Card Fraud Detection

## Overview

This repository contains my submission for **Module 20** of the **UC Berkeley Professional Certificate in Machine Learning & Artificial Intelligence**.

## Project Overview

This project focuses on using advanced machine learning methods to identify fraudulent credit card transactions.

It utilizes the publicly available **Kaggle Credit Card Fraud Detection** dataset, which contains anonymized transaction records for cardholders. The objective is to build predictive models that accurately distinguish between legitimate and fraudulent activities based on patterns in the data.

A variety of machine learning techniques—including **Logistic Regression, Decision Tree, Random Forest, AdaBoost, Gradient Boosting, XGBoost, LightGBM, and CatBoost**—are evaluated to classify transactions as either genuine or fraudulent. The purpose of this work is to improve the effectiveness of fraud detection systems while strengthening the security of credit card transaction processes.

## Business Problem

### Research Question

**How can machine learning models accurately detect fraudulent credit card transactions while minimizing false positives?**

The goal is to identify patterns that distinguish fraudulent behavior from legitimate transactions in real time.

## Why This Question is Important

Credit card fraud causes significant financial losses and impacts customer trust. Accurate fraud detection systems help financial institutions prevent fraudulent transactions in real time while minimizing inconvenience to legitimate customers.

## Dataset

Primary Dataset:
https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

The dataset contains:
- Anonymized PCA features
- Transaction amount
- Transaction time
- Fraud/Non-Fraud labels

## Methodology

- Data preprocessing
- Exploratory Data Analysis (EDA)
- Feature engineering
- Handling class imbalance
- Model training
- Hyperparameter optimization
- Model evaluation
- Feature importance analysis

## Machine Learning Models

- Logistic Regression
- Decision Tree
- Random Forest
- AdaBoost
- Gradient Boosting
- XGBoost
- LightGBM
- CatBoost

## Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC
- Precision-Recall Curve
- Confusion Matrix
- ROC Curve

Special emphasis is placed on maximizing **Recall** while maintaining high **Precision** to reduce false alarms.

## Expected Results

Tree-based and ensemble models are expected to outperform linear models by capturing nonlinear relationships within the transaction data. The objective is to maximize fraud detection while minimizing false positives.

## Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- XGBoost
- LightGBM
- CatBoost
- Jupyter Notebook

## Installation

```bash
git clone https://github.com/rsatsangi/UCBEHass-PCMLAI-MOD20.git
cd UCBEHass-PCMLAI-MOD20
pip install -r requirements.txt
jupyter notebook
```

## Author

**Rupanshu Satsangi**

- GitHub: https://github.com/rsatsangi
- LinkedIn: https://www.linkedin.com/in/rupanshusatsangi
