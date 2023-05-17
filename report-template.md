# Module 12 Report Template

## Overview of the Analysis

The purpose of this analysis is to build a model that can identify the creditworthiness of borrowers using historical lending activity data from a peer-to-peer lending services company. The data includes financial information such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. The goal is to predict the loan status, which is classified as 0 for healthy loans and 1 for high-risk loans.
* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).


## Result and Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. 

The logistic regression model trained with the original data achieved a high accuracy score of 0.9918. It performed well in predicting both healthy loans (precision: 0.91) and high-risk loans (recall: 0.93). However, the model trained with resampled data using the RandomOverSampler technique achieved a slightly lower accuracy score of 0.9854. The precision for high-risk loans decreased (precision: 0.83), but the recall increased (recall: 0.99).

Based on the results, the logistic regression model trained with the original data seems to perform better overall. It maintains a high accuracy score and balances precision and recall for both loan categories. The performance of the model depends on the problem we are trying to solve. If it is more important to accurately predict high-risk loans, the model trained with resampled data may be preferred due to its higher recall score. However, for a balanced approach, where accuracy and balanced prediction of both healthy and high-risk loans are important, the model trained with the original data is recommended.

Considering the higher accuracy score and balanced performance, the logistic regression model trained with the original data is the recommended choice for predicting credit risk in this scenario.

