# Credit-Risk-Classification
In this Challenge, I use various techniques to train and evaluate a model based on loan risk. I use a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

Overview of the Analysis:
The goal of this analysis was to assess the creditworthiness of borrowers using machine learning. We trained a logistic regression model on historical lending data to predict whether a loan is healthy (0) or high-risk (1).

The dataset included:
Financial attributes related to borrowers.
A "loan_status" column indicating loan outcome (0 = healthy, 1 = high-risk).

Machine Learning Process:
Loaded the lending_data.csv dataset.
Separated the label (loan_status) from features.
Split the data into training and testing sets using train_test_split.
Trained a LogisticRegression model with random_state=1.
Evaluated performance using a confusion matrix and classification report.

Results:
Machine Learning Model 1: Logistic Regression.
Accuracy Score: 0.99.
Precision (0 - Healthy Loan): 1.00.
Recall (0 - Healthy Loan): 0.99.
Precision (1 - High-Risk Loan): 0.85.
Recall (1 - High-Risk Loan): 0.95.

Summary:
The logistic regression model achieved 99% accuracy, indicating strong overall performance. It predicted healthy loans (0s) with perfect precision and very high recall. Notably, the model also performed well with high-risk loans (1s), achieving 85% precision and 95% recall—a rare outcome given the usual class imbalance in lending datasets.

Recommendation:
I recommend this logistic regression model for use in identifying credit risk. Its high precision and recall scores for both classes suggest it can reliably distinguish between healthy and high-risk loans. However, further monitoring is advised in a production setting to ensure consistent performance across varying borrower profiles.