### Credit Card Fraud Detection: Initial Report and Exploratory Data Analysis

#### Executive summary
Financial fraud detection is a critical challenge for banking and payment industries due to the increasing volume of digital transactions. This project develops machine learning models to identify fraudulent credit card transactions using historical transaction data. The objective is to build, optimize, and evaluate multiple supervised learning classification models capable of accurately distinguishing between legitimate and fraudulent transactions while addressing the challenges of a highly imbalanced dataset. Several algorithms are explored — including Logistic Regression, AdaBoost, Random Forest, XGBoost, LightGBM, and CatBoost — with performance assessed using fraud-appropriate metrics such as Precision, Recall, F1-score, ROC-AUC, Precision-Recall curves, and confusion matrices. The final solution provides insights into model performance, feature importance, and practical considerations for deploying machine learning-based fraud detection systems.

#### Rationale
Credit card fraud results in billions of dollars of financial losses annually and creates significant challenges for financial institutions, merchants, and customers. Traditional rule-based fraud detection systems often struggle to detect sophisticated fraud patterns because fraudulent activities continuously evolve. Machine learning provides an opportunity to analyze large volumes of transaction data, identify hidden patterns, and improve fraud detection accuracy. A robust fraud detection model can help financial organizations reduce financial losses, improve customer trust and security, detect suspicious activity faster, reduce false positives and unnecessary transaction declines, and automate fraud monitoring processes. This project investigates how machine learning algorithms can be applied to improve fraud detection effectiveness.

#### Research Question
What machine learning approach can most effectively identify fraudulent credit card transactions while maintaining a balance between detecting fraud cases and minimizing false transaction alerts?

Additional research objectives include:
- Which classification algorithms provide the best fraud detection performance?
- Which evaluation metrics are most suitable for highly imbalanced fraud datasets?
- Which transaction features contribute most significantly to fraud prediction?
- How does hyperparameter optimization improve model performance?

#### Data Sources
This project uses the publicly available Kaggle **Credit Card Fraud Detection** dataset: https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

Dataset characteristics:
- 284,807 total transactions
- 492 fraudulent transactions (highly imbalanced)
- Target variable: `Class = 0` (legitimate) or `Class = 1` (fraudulent)
- Features: transaction amount, transaction time, and 28 PCA-transformed anonymized numerical features (`V1`–`V28`)

Due to the highly imbalanced nature of the dataset, special preprocessing and evaluation techniques were applied throughout the analysis.

#### Methodology
The project follows a structured machine learning workflow:

**1. Data Exploration and Analysis** — loading and inspecting the transaction data, analyzing distributions, identifying the class imbalance, running statistical analysis, and visualizing transaction patterns.

**2. Data Preparation** — handling missing values, analyzing feature distributions, scaling numerical features, splitting data into training and testing sets, and addressing class imbalance considerations.

**3. Model Development** — training and comparing multiple classification algorithms: Logistic Regression, AdaBoost, Random Forest, XGBoost, LightGBM, and CatBoost.

**4. Model Optimization** — hyperparameter tuning via grid search / randomized search, cross-validation, and stratified sampling, tuning regularization, tree depth, learning rate, and number of estimators.

**5. Model Evaluation** — assessing models using Accuracy, Precision, Recall, F1-Score, ROC-AUC, Precision-Recall curves, Confusion Matrices, and feature importance analysis.

#### Results
Ensemble machine learning models significantly improved fraud detection performance compared with baseline approaches. Key findings:
- Tree-based ensemble models outperformed traditional linear models.
- Optimized boosting algorithms (XGBoost, LightGBM, CatBoost) achieved strong fraud detection capability by effectively capturing complex, nonlinear relationships in the transaction data.
- Recall was prioritized over overall accuracy, since correctly identifying fraudulent transactions matters more than raw accuracy in a highly imbalanced dataset.
- Feature importance analysis helped identify which transaction characteristics contribute most to fraud prediction.

Overall, the results highlight the importance of selecting evaluation metrics beyond accuracy — such as Recall, F1-score, and ROC-AUC — when working on imbalanced fraud detection problems.

#### Next steps
- Implement advanced imbalance-handling techniques such as SMOTE, ADASYN, or cost-sensitive learning
- Test deep learning approaches, including neural networks, autoencoders, or transformer-based models
- Deploy the selected model as a real-time fraud detection API
- Implement model monitoring for data drift, evolving fraud patterns, and performance degradation
- Add explainable AI techniques such as SHAP values or LIME explanations
- Integrate streaming transaction processing using cloud platforms

#### Outline of project
- [Initial Report and EDA Notebook](https://github.com/rsatsangi/UCBEHass-PCMLAI-MOD20/blob/main/CapstoneAssignment20.1-InitialReportandEDA.ipynb)
- [Data folder](https://github.com/rsatsangi/UCBEHass-PCMLAI-MOD20/tree/main/data)

##### Contact and Further Information
Rupanshu Satsangi
- GitHub: https://github.com/rsatsangi
- LinkedIn: https://www.linkedin.com/in/rupanshusatsangi
