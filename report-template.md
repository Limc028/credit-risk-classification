# Module 12 Report Template

## Overview of the Analysis

The purpose of the analysis was to develop an algorithm that can learn the the patterns in the dataset and use learning to make predictions. In this applicaiton it was to train and evaluate a model based on loan risk. A dataset of historical lending activity from peer-to-peer lending services company was made available for building a model that helps identify the creditworthiness of borrowers. 
First i had to read the `lending_data.csv` data into a Pandas DataFrame after which i created the labels set (y) from the "loan_status" columnn and also created the features (x) DataFrame from the remaining columns. The data was split into training and testing by using train_test_split.
The next step involved creating a Logistic Regressin model with the original data. Here i fitted the logistic regression model using the training data (X_train and y_train). I went on to save the predictions for the testing data labels by using the testing feature dataa (X_test) and the fitted model.


## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of the machine learning model.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
  0.9918489475856377

            precision    recall  f1-score   support

           0       1.00      0.99      1.00     18765
           1       0.85      0.91      0.88       619

    accuracy                           0.99     19384
   macro avg       0.92      0.95      0.94     19384
weighted avg       0.99      0.99      0.99     19384

Balanced accuracy score of the model = 99%. This may be attributed to the unbalanced data considering that the number of healthy loans (low-risk) by far exceeds the number og unhealthy loans (high-risk)

Precision score = 92%

Recall score = 95%
## Summary

Summarise the results of the machine learning models, and include a recommendation on the model to use, if any. 
For this analysis it is more important to predict the '0''s (healthy loan) to reduce high default rate from lendees
If the goal is to minimize the number of false positives (i.e., incorrectly classifying healthy loans as high-risk), you should focus on improving precision. In this instance, the model would be recommended
