# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

### Purpose
The purpose of this analysis is to utilise historical lending activity in file "lending_data.csv" from a peer-to-peer lending services company, to build a model that can identify the creditworthiness of borrowers.

### Data
Within the historical file, we utilise columns:
* "loan_status" - as the outcome to identify the creditworthiness of borrowers. "0" being a healthy loan and "1" a high risk loan.
* The other columns are the feature variables in which the machine learning process will be trained and tested on in predicting the "loan_status" outcome.

### Machine Learning Process
Utilising logistic regression modelling:
* "Train_test_split()" function was used to split the file data into subsets for training or testing.
* "LogisticRegression()" function was used to train the machine learning model using the training data subset, by assessing the feature variables and define a percentage probabiltty of whether the loan is healthy or high risk.
* "Predict()" function was then used on the test data subset to predict the outcome.
* "confusion_matrix()" and "classification_report()" function is used to measure the sucess of a model and provide the precision, recall and accuracy of the machine learning model.

## Results

### Accuracy, Precision and Recall
The model is accurate 99% of the time.

### Precision 
Although the model is accurate, the precision and recall for healthy loans is 100% correct whereas at-risk loans is 87% and 89% respectively. Although 87% and 89% is still high, the number of good loans can be seen outweighing the number of at-risk loans and having the biggest impact on accuracy.

It can be seen that there is high precision - therefore a low false positive rate, and high recall rate - therefore a low false negative rate. In the case of healthy loans, it's 100%.


## Summary

As per the above, the accuracy, precision and recall percentages are high - although the identificaiton of at-risk loans precision/recall is lower than the healthy ones.

The high risk loans are the most important to identify, and as the model's prediction of at-risk loans are high, it would be recommended to implement this model during the company's assessment process of providing a loan. 
