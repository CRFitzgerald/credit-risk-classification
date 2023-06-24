# credit-risk-classification
## Overview of the Analysis

The purpose of this analysis is to train and evaluate a model based on loan risk. I used a dataset of historical lending activity from a peer-to-peer lending services company. Using this data, I am predicting the creditworthiness of borrowers. The target variable (labels set) was loan status. 
* A score of 0 means the loan is healthy, whereas a score of 1 means that it has a high risk of defaulting.
  
Features included loan size,	interest rate,	borrower income,	debt-to-income,	number of accounts, derogatory marks, and	total debt.

Stages of Machine Learning:
1. Reading in the data
2. Splitting the data into Training and Testing sets
3. Fitting data to models
4. Using the models to create predictions
5. Evaluating the model's performance through confusion matrices and classifications reports.
   
I went through the above procedure with a Logistic Regression Model with original data as well as with resampled data.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

### Machine Learning Model 1: Logistic Regression using Original Data
  * Accuracy: 99%
  * Precision: 100% for Healthy Loans, but only 87% for Unhealthy Loans
  * Recall scores: 100% for Healthy Loans, but only 89% for Unhealthy Loans

### Machine Learning Model 2: Logistic Regression using Resampled Data
 * Accuracy: 99%
 * Precision: 99% for both Healthy Loans and Unhealthy Loans
 * Recall scores: 199% for both Healthy Loans and Unhealthy Loans
   
## Summary

Logistic Regression using the originl data performed very slightly better in predicting Healthy Loan labels. However, it performed significantly worse at predicting Unhealthy Loans. Logistic Regression using resampled  data performed much better at predicting Unhealthy labels and almost as well at predicting Healthy labels.
I recommend using the Logistic Regression model with resampled data. It will prevent lenders from taking unecessary risks and borrowers from overextending themselves. 
