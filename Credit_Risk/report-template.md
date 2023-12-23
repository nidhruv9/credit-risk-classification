# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.

The Aim of the analysis is to find out if Logistic Reression model can be accurate to predict healthy loans (class `0`) versus high risk loans (class `1`) using original data versus resampled data to increase the size of the minority class


* Explain what financial information the data was on, and what you needed to predict.

loan_status is the predictions.

* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).

Value Counts 

Original data:

Healthy loans (`0`)    ---- >   75036

High risk loans (`1`)    ---- >     2500



Oversampled:

Healthy loans (`0`)    ---- >    56271

High risk loans (`1`)    ---- >    56271

* Describe the stages of the machine learning process you went through as part of this analysis.

1. Prepare the Data.
2. Separate the data to features (columns or X) and outcome (labels or y).
3. split the data in training and testing sets.
4. picking the logistic regression machine learning model.
5. fit model with the training data.
6. use the model to make predictions with the test data so 25% default test data to be evaluated.
7. Evaluate the predictions by comparing the confusion matrices and classification reports.


* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

SKLearn Logistic Regression
train_test_split
confusion_matrix
classification_report

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 
  * Accuracy: 0.99
  * Precision class `0`: 1.00 ,  Precision class `1`: 0.85 
  * Recall scores : class `0`: 0.99, class `1`: 0.91



* Machine Learning Model 2:
  * Description of Model 2 
  * Accuracy: 0.99
  * Precision class `0`: 1.00 ,  Precision class `1`: 0.84 
  * Recall scores : class `0`: 0.99, class `1`: 0.99

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?

Overall Logistic Regression model performed well especially predicting the outcome class `0` (healthy loans). Both the precisions and recalles were extremely high.



* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

for the class `1` (high risk loans), the model's precision is 0.84 and recall is 0.91. This indiactes the model more often gives false positives than false negatives.

Given the information it appears that logistic regression model does a great job at predicting both healthy and high risk loans given the features that are used to training set data.



* If you do not recommend any of the models, please justify your reasoning.

Although the logistic regression model appears promising, it would need to be evaluated against different data sets to confirm that it should be put in to use for predicting health status of loans.

