# Module 12 Report Template

# Credit Risk Analysis Report

# Overview of the Analysis

As part of this analysis/challenge, performance of various machine learning models in assessing credit risk based on financial data were assessed.

### In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:
####  Explain the purpose of the analysis.
The main goal was to assess various supervised machine learning models in predicting the likelihood of loan default based on customer financial details. Model performances were assessed based on how well the models were able to make predictions based on test and train data.

#### Explain what financial information the data was on, and what you needed to predict.
The dataset included several customer financial details, such as interest rate, borrower income, debt-to-income ratio, loan size, number of accounts, derogatory marks, total debt, and a classification recorder, loan status. The key task was to train a classification machine learning model on a train dataset and use the trained model to predict in decision process, i.e. to decide whether a loan application is a healthy (0) or high-risk (1).

#### Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
Accuracy of model, balanced F-score, precision of model, part of confusion matrix and classification report were assessed, in order to evaluate the performance of machine learning models. Variables such as health of loan, risk of default, financial conditions of customer such as debt-to-income ratio, interest rates were also used in the assessment.

#### Describe the stages of the machine learning process you went through as part of this analysis.
The process involved data processing using Pandas, standardising the data using StandardScaler function, converting data into features and labels, splitting the data into training and testing sets, and then performing train and test the machine learning models. Finally using the trained machine learning model, prediction was performed.

#### Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).
Initially Classification Machine Learning Model, Logistic Regression was used for predicting risk classification due to effectiveness in binary classification tasks. Later, performance of Linear Support Vector Machines (SVM), Decision Trees, Random Forests and k-nearest Neighbours machine learning models were tested on test data.

## Results
Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

### Machine Learning Model 1: Logistic Regression
*Accuracy*: The model achieved an accuracy of 99.3%, which is exceptionally high and indicates a high level of overall correctness in its predictions.
*Precision for Healthy Loans (0)*: 100%, showing excellent reliability in predicting low-risk loans.
*Recall for Healthy Loans (0)*: 100%, indicating the model's ability to correctly identify the majority of low-risk loans.
*Precision for High-Risk Loans (1)*: 87%, which is good and indicates the model's reliability in identifying loans at high risk of default.
*Recall for High-Risk Loans (1)*: 90%, suggesting that the model can correctly identify a high percentage of high-risk loans.

*Harmonic mean of precision and recall score (F1)* for Healthy (100%) and High-risk loans (89%) were also good indicating that model is suitable for predicting the high-risk loans.

### Machine Learning Model 2: Support Vector Machines

*Accuracy*: The model achieved an accuracy of 99.3%, similar to Logistic Regression Model.
*Precision for Healthy Loans (0)*: 100%, showing excellent reliability in predicting low-risk loans.
*Recall for Healthy Loans (0)*: 99%, indicating the model's ability to correctly identify the majority of low-risk loans.
*Precision for High-Risk Loans (1)*: 84%, which is good and indicates the model's reliability in identifying loans at high risk of default.
*Recall for High-Risk Loans (1)*: 97%, suggesting that the model can correctly identify a high percentage of high-risk loans.

*Harmonic mean of precision and recall score (F1)* for Healthy (100%) and High-risk loans (90%) were also good indicating that model is suitable for predicting the high-risk loans.

### Machine Learning Model 3: Decision Trees Model
*Accuracy*: The model achieved an accuracy of 99.0%, indicating a high level of overall correctness in its predictions.
*Precision for Healthy Loans (0)*: 99%, showing excellent reliability in predicting low-risk loans.
*Recall for Healthy Loans (0)*: 100%, indicating the model's ability to correctly identify the majority of low-risk loans.
*Precision for High-Risk Loans (1)*: 84%, which is good and indicates the model's reliability in identifying loans at high risk of default.
*Recall for High-Risk Loans (1)*: 83%, suggesting that the model can correctly identify a high percentage of high-risk loans.

*Harmonic mean of precision and recall score (F1)* for Healthy (99%) and High-risk loans (84%) were also good indicating that model is suitable for predicting the high-risk loans.

### Machine Learning Model 4: Random Forest Model

*Accuracy*: The model achieved an accuracy of 99.0%, indicating a high level of overall correctness in its predictions.
*Precision for Healthy Loans (0)*: 100%, showing excellent reliability in predicting low-risk loans.
*Recall for Healthy Loans (0)*: 99%, indicating the model's ability to correctly identify the majority of low-risk loans.
*Precision for High-Risk Loans (1)*: 85%, which is good and indicates the model's reliability in identifying loans at high risk of default.
*Recall for High-Risk Loans (1)*: 89%, suggesting that the model can correctly identify a high percentage of high-risk loans.

*Harmonic mean of precision and recall score (F1)* for Healthy (100%) and High-risk loans (87%) were also good indicating that model is suitable for predicting the high-risk loans.

### Machine Learning Model 5: k-nearest neighbours Model

*Accuracy*: The model achieved an accuracy of 99.2%, indicating a high level of overall correctness in its predictions.
*Precision for Healthy Loans (0)*: 99%, showing excellent reliability in predicting low-risk loans.
*Recall for Healthy Loans (0)*: 100%, indicating the model's ability to correctly identify the majority of low-risk loans.
*Precision for High-Risk Loans (1)*: 93%, which is good and indicates the model's reliability in identifying loans at high risk of default.
*Recall for High-Risk Loans (1)*: 84%, suggesting that the model can correctly identify a high percentage of high-risk loans.

*Harmonic mean of precision and recall score (F1)* for Healthy (100%) and High-risk loans (88%) were also good indicating that model is suitable for predicting the high-risk loans.

## Summary
Summarise the results of the machine learning model, and include a recommendation on the model to use, if any. For example:

#### Which one seems to perform best? How do you know it performs best?
Of all the Machine Learning models, Classification model, Logistic Regression model demonstrated strong performance in identifying both healthy and high-risk loans as datasets were of logical in nature. Its high accuracy, in combination with excellent precision and recall for healthy loans and good scores for high-risk loans, makes it a valuable tool in customer loan application assessments. It is recommended to deploy this model for credit risk assessment in a lending institution where the outcomes are to classify the loans/applications into low-risk and high-risk categories.

#### Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s?)
A balance between high-risk loans and healthy loans is required and it depends on the risk assessment analysis undertaken by the lending institutes. Performance of a model depends on the risk tolerance levels of lending institutes, as emphasizing on any side will certainly have negative impacts such as higher high-risk loans or low amount of loans, if high emphasis is given for healthy loans. 

If you do not recommend any of the models, please justify your reasoning.
