# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

Explain the purpose of the analysis: Resolve classification problem of data when making prediction through the use of supervised learning models. 

Explain what financial information the data was on, and what you needed to predict: Financial data was on historical lending activity including loan size, interest rates, borrower income, debt to income ration, number of accounts, derogatory remarks, total debt, and loan status. We needed to predict wether or not a loan presents high risks.

 Provide basic information about the variables you were trying to predict (e.g., `value_counts`): model was trying to predict wether or not borrower would be able to maitain a desirable loan status. Prediction were made based on data provided of  75036 healthy loans and  2500 high risk loans
 
Describe the stages of the machine learning process you went through as part of this analys: We split the data into training and testing sets then created a logistic regression model with the original data. Next we resampled the data to make sure it is not imbalanced so that we can predict a logistic regression model with resampled data.

Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method): We created a fit Logistic regression using training data then we used a random oversampler module to make sure we bring data to an equal point


## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

Machine Learning Model 1: logistic regression model with original data
   Accuracy: 0.9918
   Precision: 0.92
   Recall scores:0.95



Machine Learning Model 2: logistic regression with resampled training data
   Accuracy: 0.9938
   Precision: 0.92
   Recall scores: 0.99

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
Which one seems to perform best? How do you know it performs best? Logistic regression with resampled data seems to perform best because the imbalanced issue of the data was taken care of. We can tell it performs best because its evaluation yields better results. I would recommend this model over the other.

Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
Performance depend on the problem we are trying to solve as we want to accurately predict healthy loans and high risks loans instead of predicting more of one over the other.

If you do not recommend any of the models, please justify your reasoning.
I do recommend using logistic regression with resampled data when facing a classification problem (in our case solving the imbalance using oversampler).
