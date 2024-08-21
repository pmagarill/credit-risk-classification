credit-risk-classification
Overview of the Analysis
The purpose of this analysis was to evaluate the borrower credit worthiness from peer-to-peer lending services.
The original data consisted of a CSV file with 77.5K lines. The loan status is what needs to be predicted. The information in the remaining columns is used to predict this.
The loan status consisted of two target variables: 0 to indicate a healthy loan, and 1 to indicate high risk of defaulting.
This was done by creating label sets, splitting the data into train and test sets, creating a logistic regression model, fitting data into the model, making predictions, and evaluating performance.
The primary method used was Logistic Regression.
Results
Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

Machine Learning Model:

              precision    recall  f1-score   support

           0       1.00      0.99      1.00     18765
           1       0.85      0.91      0.88       619

    accuracy                           0.99     19384
   macro avg       0.92      0.95      0.94     19384
weighted avg       0.99      0.99      0.99     19384

Summary
The logistic regression model excels at predicting healthy loans, achieving a precision of 1.00 and a recall of 0.99. For risky loans, the model still performs well, with a precision of 0.85 and a recall of 0.91. Overall, the model's accuracy is very high at 99%.

The lower precision and recall for risky loans may be due to the imbalanced nature of the dataset. There were only 619 instances of high risk loans, as opposed to 18,765 instances of healthy loans. The model has fewer examples of high-risk loans to learn from than if it was more balanced.