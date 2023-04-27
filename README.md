# credit-risk-classification

# Report 

## Overview of the Analysis

The purpose of this analysis is to build a model that can identify the creditworthiness of loan borrowers, using a dataset of historical lending activity from a peer-to-peer lending services company. The dataset contained information on loan size, interest rate, borrower incom, debt to income ratio, number of accounts, derogatory marks, total debt, loan status.

We divided our dataset to 2 subsets: training set and testing set. Training set is used to train the machine learning model. The testing set is used to introduced unknown data to the model and get the predictions for it. After we got the predictions, we calculated the accuracy rating, confusion matrix, and classification report to analyse the effectiveness of each particular model. 

As a part of our project, we used LogisticRegression method as well as resampling method. 

Logistic Regression methos is widely used algorithm got binary classification tasks. Logistic Regression models the relationship between a set of input variables and a binary target variable by estimating the probabilities of the target variable belonging to each class.
Resampling is a technique in machine learning and statistics that involves creating new datasets by sampling from an existing dataset. Random resampling provides a technique for rebalancing the class distribution for an imbalanced dataset. For our dataset we used Random Oversampling: Randomly duplicate examples in the minority class, providing more balanced class distribution. 

<hr>

## Results

<b>Machine Learning Model 1:</b>
  The logistic regression model has an overall accuracy rating of 99,24%
Healthy Loan:
- Precision and recall both equal 1.00 meaning that the model identified all the possible healthy loans and out of all identified healthy loans 100% was correct. 
High-Risk Loan: 
- Precision is 0.87, meaning out of all predicted high-risk loans, 87% were correct predictions (which means that there are false negatives present). Recall being 0.89 suggests out of all actual high-risk loans. 89% were identified by the clasifier, leaving us with 11% false positives cases. 


<b>Machine Learning Model 2:</b>
  The logistic regression model has an overall accuracy rating of 99,52%, which is higher than the previous model. 
Healthy Loan:
- Precision and recall both equal 1.00 meaning that the model identified all the possible healthy loans and out of all identified healthy loans 100% was correct. 
High-Risk Loan: 
- Precision is 0.94, meaning out of all predicted high-risk loans, 94% were correct predictions (which means that there is 6% false negatives present). Recall being 1.00 suggests out of all actual high-risk loans. 100% were identified by the clasifier, which makes this model more suitable for out needs. 

<hr> 

## Summary

For our goal it is more vital to identify all high-risk loans. Keeping that in mind, we would suggest using the second machine learning model, since the recall score is shown to be 1.00, meaning the model identified 100% high-risk loans out of all actual high-risk loans. Also, it should be noted that our datasets are imbalanced (one class has significantly more samples than the other), so it is a good practice to pay attention to the f1 score, otherwise known as a harmonic mean. It provides a balanced measure of a model's performance, particularly when dealing with imbalanced datasets. F1 score of individual high-risk loan and overall f1 score have better values in the second model
(0,88/0,99 vs 0,93/1.00), providing our suggestion to use the second model with more support. 

