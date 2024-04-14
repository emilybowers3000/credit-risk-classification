# Module 12 Credit Analysis Report 

## Overview of the Analysis

The purpose of the analysis was to build machine learning models to predict loan statuses based on various financial features. The dataset contained information about loan applicants, including loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, total debt, and loan status.

The goal was to predict whether a loan would be healthy (0) or high-risk (1) based on the provided financial information. The loan status variable had two categories: healthy loans (0) and high-risk loans (1).

Here's an overview of the stages of the machine learning process:

Data Preprocessing: Initially, I separated the data into labels (y) and features (X). The labels were taken from the loan_status column, while the features were derived from the remaining columns in the dataset.

Train-Test Split: The data was split into training and testing sets using the train_test_split function from sklearn. A random state of 1 was assigned to ensure reproducibility.

Model Selection and Training: For this analysis, a logistic regression model was chosen for its simplicity and interpretability. The LogisticRegression module from sklearn was imported, and an instance of the logistic regression model was instantiated with a random state parameter of 1. The model was then fitted using the training data.

Model Evaluation: The performance of the trained model was evaluated using the testing data. Confusion matrix and classification report were generated to assess the model's performance metrics such as precision, recall, and F1-score for both healthy and high-risk loans.

Throughout the analysis, the logistic regression algorithm was used as the primary method for predicting loan statuses. The model demonstrated high accuracy, precision, and recall for both healthy and high-risk loans, indicating its effectiveness in predicting loan statuses based on the provided financial features.


## Results

Machine Learning Model 1 (Logistic Regression):
Accuracy: 99%
Precision (Healthy Loans): 100%
Precision (High-Risk Loans): 85%
Recall (Healthy Loans): 99%
Recall (High-Risk Loans): 91%
The logistic regression model achieved an accuracy of 99%, indicating that it correctly predicted loan statuses for the vast majority of the testing data. For healthy loans, the precision and recall were both high at 100% and 99%, respectively, suggesting that the model effectively identified and correctly classified healthy loans. For high-risk loans, while the precision was slightly lower at 85%, the recall remained relatively high at 91%, indicating that the model could identify a substantial portion of high-risk loans, although with some misclassifications.

## Summary

Based on the results of the machine learning models, the logistic regression model appears to perform the best among the models evaluated. It achieved an accuracy score of 99%, indicating a high level of overall correctness in predicting loan statuses.

However, the performance of the model varies depending on the specific problem we are trying to solve. If the primary focus is on identifying healthy loans (label 0), the logistic regression model performs exceptionally well, with both precision and recall scores of 100% and 99%, respectively. This means that it accurately identifies and classifies the vast majority of healthy loans.

On the other hand, if the priority is to predict high-risk loans (label 1), the model's performance is slightly lower but still relatively strong. The precision for high-risk loans is 85%, indicating that when the model predicts a loan as high-risk, it is correct 85% of the time. The recall for high-risk loans is 91%, suggesting that the model can identify the majority of high-risk loans in the dataset.

Considering the trade-offs between precision and recall, as well as the specific objectives of the analysis, the logistic regression model is recommended for this scenario. Its high accuracy and balanced performance in predicting both healthy and high-risk loans make it a suitable choice for classification tasks in this context.