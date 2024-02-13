# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
The goal is to determine if Logistic Rgeression model can be accurate to predict healthy loans versus high risk loans using original data versus resampled data to increase the size of the minority class.

* Explain what financial information the data was on, and what you needed to predict.
Loan_status is the prediction.

* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
values_counts
0     75036
1     2500

oversampled
0     56271
1     56721

* Describe the stages of the machine learning process you went through as part of this analysis.
1. Prepare data
2. Separate the data to features aka columns which X and y is the outcome  or aka labels
3. train_test_split
4. Pick the ml model for classification so LogisticRegression
5. Fit the model with training data
6. Use the model to make predictions with the test data so 25% default test data to be evaluated
7. Evaluate the predictions comparing metrics, confusion metric, classification report.

* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).
SKLearn LogisticRegression
train_test_split
confusion_matrix
classification_report

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 
  * Accuracy: 0.99 
  * Precision Class 0: 1.00, Class 1: 0.85
  * Recall Class 0: 0.99, Class 1: 0.91



* Machine Learning Model 2:
  * Description of Model 2 
  * Accuracy: 0.99 
  * Precision Class 0: 1.00, Class 1: 0.84
  * Recall Class 0: 0.99, Class 1: 0.91

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
Overall Logistic Regression model performed well especially for the prediction of the outcome 0 healthy loans for class 0. Both the precision and recall were extremely high.

* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
For 1 class high risk loans the model precision is 0.84 and the recall is 0.91. This indicates that the model often gives false positives tahn false negatives.

Given the info, it appears logistic regression models do a great job at predicting both healthy and high risk laons given the features used for training data set.

If you do not recommend any of the models, please justify your reasoning.
