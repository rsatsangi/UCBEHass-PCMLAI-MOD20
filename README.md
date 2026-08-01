# UC Berkeley Professional Certificate in Machine Learning & AI
## Module 20 – Credit Card Fraud Detection

## Overview

This repository contains my submission for **Module 20** of the **UC Berkeley Professional Certificate in Machine Learning & Artificial Intelligence**.

## Executive summary

Financial fraud detection is a critical challenge for banking and payment industries due to the increasing volume of digital transactions. This project focuses on developing machine learning models to identify fraudulent credit card transactions using historical transaction data.

The objective of this project is to build, optimize, and evaluate multiple supervised learning classification models capable of accurately distinguishing between legitimate and fraudulent transactions while addressing the challenges of highly imbalanced datasets.

The project explores multiple machine learning algorithms, including Logistic Regression, AdaBoost, Random Forest, XGBoost, LightGBM, and CatBoost. Model performance is evaluated using appropriate fraud detection metrics such as Precision, Recall, F1-score, ROC-AUC, Precision-Recall curves, and confusion matrices.

The final solution provides insights into model performance, feature importance, and practical considerations for deploying machine learning-based fraud detection systems.

---

## Rationale

Why should anyone care about this question?

Credit card fraud results in billions of dollars of financial losses annually and creates significant challenges for financial institutions, merchants, and customers. Traditional rule-based fraud detection systems often struggle to detect sophisticated fraud patterns because fraudulent activities continuously evolve.

Machine learning provides an opportunity to analyze large volumes of transaction data, identify hidden patterns, and improve fraud detection accuracy. A robust fraud detection model can help financial organizations:

- Reduce financial losses caused by fraudulent transactions
- Improve customer trust and security
- Detect suspicious activities faster
- Reduce false positives and unnecessary transaction declines
- Automate fraud monitoring processes

This project investigates how machine learning algorithms can be applied to improve fraud detection effectiveness.

---

## Research Question

What machine learning approach can most effectively identify fraudulent credit card transactions while maintaining a balance between detecting fraud cases and minimizing false transaction alerts?

Additional research objectives include:

- Which classification algorithms provide the best fraud detection performance?
- Which evaluation metrics are most suitable for highly imbalanced fraud datasets?
- Which transaction features contribute most significantly to fraud prediction?
- How does hyperparameter optimization improve model performance?

---

## Data Sources

The project uses a publicly available credit card transaction dataset containing historical transaction records.

Dataset characteristics:

- Source: Public Credit Card Fraud Detection Dataset
- Number of transactions: 284,807
- Fraudulent transactions: 492
- Target variable:
  - `Class = 0` → Legitimate transaction
  - `Class = 1` → Fraudulent transaction

The dataset includes:

- Transaction amount
- Transaction time
- PCA-transformed numerical features (`V1` - `V28`)
- Fraud classification label (`Class`)

Due to the highly imbalanced nature of the dataset, special preprocessing and evaluation techniques were applied.

---

## Methodology

The project follows a structured machine learning workflow:

### 1. Data Exploration and Analysis

- Load and inspect transaction data
- Analyze data distributions
- Identify class imbalance
- Perform statistical analysis
- Visualize transaction patterns

### 2. Data Preparation

- Handle missing values
- Analyze feature distributions
- Scale numerical features
- Split data into training and testing datasets
- Address class imbalance considerations

### 3. Model Development

Multiple classification algorithms were developed and compared:

- Logistic Regression
- AdaBoost Classifier
- Random Forest Classifier
- XGBoost Classifier
- LightGBM Classifier
- CatBoost Classifier

### 4. Model Optimization

Hyperparameter tuning was performed using:

- Grid Search / Randomized Search
- Cross-validation
- Stratified sampling techniques

Optimized models included:

- Regularization tuning
- Tree depth optimization
- Learning rate optimization
- Number of estimators optimization

### 5. Model Evaluation

Models were evaluated using fraud-focused performance metrics:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC Score
- Precision-Recall Curve
- Confusion Matrix
- Feature Importance Analysis

---

## Results

The analysis demonstrated that ensemble machine learning models significantly improved fraud detection performance compared with baseline approaches.

Key findings:

- Tree-based ensemble models performed better than traditional linear models.
- Optimized boosting algorithms achieved strong fraud detection capability.
- Recall was prioritized because identifying fraudulent transactions is more important than overall accuracy in highly imbalanced datasets.
- Feature importance analysis helped identify transaction characteristics contributing most to fraud prediction.

Model comparison showed that optimized ensemble models such as:

- XGBoost
- LightGBM
- CatBoost

provided strong predictive performance by effectively capturing complex relationships within transaction data.

The final model evaluation highlights the importance of selecting appropriate metrics beyond accuracy for fraud detection problems.

---

## Next steps

Future improvements could include:

- Implementing advanced imbalance handling techniques:
  - SMOTE
  - ADASYN
  - Cost-sensitive learning

- Testing deep learning approaches:
  - Neural Networks
  - Autoencoders
  - Transformer-based models

- Deploying the selected model as a real-time fraud detection API

- Implementing model monitoring for:
  - Data drift detection
  - Fraud pattern changes
  - Performance degradation

- Adding explainable AI techniques:
  - SHAP values
  - LIME explanations

- Integrating streaming transaction processing using cloud platforms.

---

## Outline of project

- Exploratory Data Analysis Notebook

- Data Preprocessing and Feature Engineering Notebook

- Machine Learning Modeling and Evaluation Notebook

  [Click Here](./CapstoneAssignment20.1-InitialReportandEDA.ipynb)

---

## Author

**Rupanshu Satsangi**

- GitHub: https://github.com/rsatsangi
- LinkedIn: https://www.linkedin.com/in/rupanshusatsangi
