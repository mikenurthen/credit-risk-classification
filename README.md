# credit-risk-classification
## Module 20 Challenge

In this Homework Challenge, I used the activities from class days 01 and 02 and review of the lectures from both days to work through completing the assignment.

# Credit Risk Analysis Report
## Overview of the Analysis
The purpose of the analysis was to apply machine learning against a dataset of historic lending data to help predict the creditworthiness of future borrowers. In the historic lending data, a loan status of 0 indicated that the loan remained in good standing, and a value of 1 indicated that the loan has a high-risk of defaulting. We then build a model that would train on a subset of the historic lending data, make predictions on whether those loans were healthy or high-risk, and then compared those predictions

## Results
<b>Accuracy:</b> The ratio of correctly predicted observations to the total number of observations is 99%, which means the model has a high degree of accuracy in predicting healthy loans versus high-risk loans.

<b>Precision:</b> The proportion of positive predictions that are actually correct. 100% for healthy loans, 87% for high-risk loans. Precision is important in that out of all loans that will be high-risk, we want a model to correctly predict those loans as being high-risk.

<b>Recall:</b> The proportion of correctly predicted positive observations to all predicted observations for that class. High recall correlates to a more comprehensive output and a low false negative rate. 100% for healthy loans, 89% for high-risk. This means for all loans which were healthy, the model correctly classified 100% of those as healthy, and for all loans that were high-risk, the model correctly classified 89% of those as being high-risk.

## Summary
The model demonstrates an overall accuracy of 99%, indicating the logistic regression model predicts the labels very well. It correctly predicts Healthy Loan's 100% of the time, and correctly predicts high-risk loans 87% of the time. Overall with a 99% accuracy, I would justify using this model to correctly predict the creditworthiness of future borrowers. We can also see that the original DataFrame had an imbalance of healthy versus high-risk loans in which to train the model. Out of 77,536 loans, just 2,500 were high-risk.
________________________________________
________________________________________
## Instructions
The instructions for this Challenge are divided into the following subsections:
* Split the Data into Training and Testing Sets
* Create a Logistic Regression Model with the Original Data
* Write a Credit Risk Analysis Report

## Split the Data into Training and Testing Sets
Open the starter code notebook and use it to complete the following steps:
  1. Read the lending_data.csv data from the Resources folder into a Pandas DataFrame.
  2. Create the labels set (y) from the “loan_status” column, and then create the features (X) DataFrame from the remaining columns.

NOTE: A value of 0 in the “loan_status” column means that the loan is healthy. A value of 1 means that the loan has a high risk of defaulting.

  3. Split the data into training and testing datasets by using train_test_split.
## Create a Logistic Regression Model with the Original Data
Use your knowledge of logistic regression to complete the following steps:
1. Fit a logistic regression model by using the training data (X_train and y_train).
2. Save the predictions for the testing data labels by using the testing feature data (X_test) and the fitted model.
3. Evaluate the model’s performance by doing the following:
    - Generate a confusion matrix.
    - Print the classification report.
4. Answer the following question: How well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels?

## Write a Credit Risk Analysis Report
Write a brief report that includes a summary and analysis of the performance of the machine learning models that you used in this homework. You should write this report as the README.md file included in your GitHub repository.

Structure your report by using the report template that Starter_Code.zip includes, ensuring that it contains the following:
  - <b> An overview of the analysis:</b> Explain the purpose of this analysis.
  - <b> The results:</b> Using a bulleted list, describe the accuracy score, the precision score, and recall score of the machine learning model.
  - <b> A summary:</b> Summarize the results from the machine learning model. Include your justification for recommending the model for use by the company. If you don’t recommend the model, justify your reasoning.
