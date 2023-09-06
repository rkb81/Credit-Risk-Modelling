**Overview of the Analysis**

**Purpose of the Analysis:**

The purpose of this analysis is to evaluate the performance of machine learning models for predicting loan statuses, specifically healthy and high-risk loans. The analysis addresses the imbalanced classes and assesses the models' abilities to distinguish between healthy loans (class 0) and high-risk loans (class 1). Two machine learning models are compared, one using the original data and another using resampled training data to address class imbalance.

**Financial Information and Prediction:**

The data contains financial information related to loans, including loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. The goal is to predict whether a loan is healthy (class 0) or high-risk (class 1) based on this financial information.

**Variables and Class Distribution:**

- Class 0 (Healthy Loans): 15,001 samples
- Class 1 (High-Risk Loans): 507 samples

**Stages of the Machine Learning Process:**

- Data Loading and Exploration
- Data Splitting into Training and Testing Sets
- Model 1: Logistic Regression with Original Data
- Model 2: Logistic Regression with Resampled Training Data
- Evaluation of Model Performance

**Methods Used:**

- Logistic Regression for both Model 1 and Model 2.
- Resampling using RandomOverSampler to address class imbalance for Model 2.

**Results**

**Machine Learning Model 1 (Original Data):**

**Classification Report (Model 1):**

- Balanced Accuracy Score (Model 1): 0.9521
- Precision for Class 0 (Healthy Loans): 1.00
- Precision for Class 1 (High-Risk Loans): 0.86
- Recall for Class 0 (Healthy Loans): 1.00
- Recall for Class 1 (High-Risk Loans): 0.91

**Machine Learning Model 2 (Resampled Data):**

**Classification Report (Model 2):**

- Balanced Accuracy Score (Model 2): 0.9942
- Precision for Class 0 (Healthy Loans): 1.00
- Precision for Class 1 (High-Risk Loans): 0.85
- Recall for Class 0 (Healthy Loans): 0.99
- Recall for Class 1 (High-Risk Loans): 0.99

**Summary**

- Model 2, which uses resampled training data to address class imbalance, outperforms Model 1.
- Model 2 achieves a higher balanced accuracy score (0.9942) compared to Model 1 (0.9521).
- Model 2 maintains high precision for healthy loans (class 0) while improving precision for high-risk loans (class 1) compared to Model 1.
- Model 2 also achieves excellent recall scores for both classes, indicating strong performance in identifying loan statuses.

**Recommendation:**
Based on the results, Model 2, which uses logistic regression with resampled training data, is recommended for predicting loan statuses. It is superior to model 1 in terms of balanced accuracy score, precision and recall for high risk loans, consistency in performance and class imbalance handling. Model 2 is the better choice for balanced performance.
