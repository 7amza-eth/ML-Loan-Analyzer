# Module 12 Report Template

## Overview of the Analysis

In this analysis, loan data was analyized to determine whether a loan was healthy or high risk. The status of the loan was predicted using a Logistic Regression model fit using the provided data. The original test data was imbalanced by a ratio of 30:1 healthly loans vs high risk loans. Due to this imbalance, 2 seperate prediction models were used: one with the original data and one that was balanced using an oversampling model. This was done to test the accuracy and precision difference between using an imbalanced and balanced data set.

## Results

* Logistic Regression Model 1 predicting high-risk loans using the imbalanced data set:
  * Accuracy: 0.95
  * Precision: 0.85
  * Recall: 0.91
  * F1 Score: 0.88

* Logistic Regression Model 2 predicting high-risk loans using the oversampled balanced data set:
  * Accuracy: 0.99
  * Precision: 0.84
  * Recall: 0.99
  * F1 Score: 0.91

## Summary

The model using the oversampled data performed better, this can be seen by the higher recall and f1 score when predicting a high-risk loan. I would recommend using the model fit with the oversampled data as it performed best for the problem that we are trying to solve (the prediction of '1's)

## dependencies
RandomOverSampler from imblearn.over_sampling, LogisticRegression from sklearn.linear_model, train_test_split from sklearn.model_selection, sklearn.metrics, numpy, pandas, pathlib

