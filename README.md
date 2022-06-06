# Credit Risk Analysis

This Project builds a model that can identify the creditworthiness of borrowers.
* Financial information/Resources:
lending_data.csv file is used to predict loan status in this project. 
* Information about the variables :
  `value_counts`: Count the distinct values of the resampled labels data
* The stages of the machine learning process:
  1. Split the Data into Training and Testing Sets
  2. Create a Logistic Regression Model with the Original Data
  3. Predict a Logistic Regression Model with Resampled Training Data

* The logistic regression model is used to compare two versions of the dataset: the original dataset and resample the data by using the RandomOverSampler module from the imbalanced-learn library. In this project, We calculate the count of the target classes, train a logistic regression classifier, calculate the balanced accuracy score, generate a confusion matrix, and generate a classification report.



## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1: logistic regression model with original data
                precision    recall  f1-score   support

           0       1.00      0.99      1.00     18765
           1       0.85      0.91      0.88       619

    accuracy                           0.99     19384
   macro avg       0.92      0.95      0.94     19384
weighted avg       0.99      0.99      0.99     19384


* Machine Learning Model 2:logistic regression model with resampled training data
                  pre       rec       spe        f1       geo       iba       sup

          0       1.00      0.99      0.99      1.00      0.99      0.99     18765
          1       0.84      0.99      0.99      0.91      0.99      0.99       619

avg / total       0.99      0.99      0.99      0.99      0.99      0.99     19384


The logistic regression model with original data performs better since it accuracy score is higher than the other model.
