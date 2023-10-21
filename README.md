# Credit-Card-Fraud-Detection-using-ML
This project uses machine learning to detect fraudulent credit card transactions. The project uses the Kaggle Credit Card Fraud Detection dataset, which contains 284,807 transactions made by European cardholders in September 2013. The dataset is highly unbalanced, with only 492 frauds out of 284,807 transactions.
About Dataset
Context It is important that credit card companies are able to recognize fraudulent credit card transactions so that customers are not charged for items that they did not purchase.

Content The dataset contains transactions made by credit cards in September 2013 by European cardholders. This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) accounts for 0.172% of all transactions.

It contains only numerical input variables which are the result of a PCA transformation. Unfortunately, due to confidentiality issues, we cannot provide the original features and more background information about the data. Features V1, V2, … V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'. Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset. The feature 'Amount' is the transaction Amount, this feature can be used for example-dependent cost-sensitive learning. Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise.

Given the class imbalance ratio, we recommend measuring the accuracy using the Area Under the Precision-Recall Curve (AUPRC). Confusion matrix accuracy is not meaningful for unbalanced classification.

Update (03/05/2021) A simulator for transaction data has been released as part of the practical handbook on Machine Learning for Credit Card Fraud Detection - https://fraud-detection-handbook.github.io/fraud-detection-handbook/Chapter_3_GettingStarted/SimulatedDataset.html. We invite all practitioners interested in fraud detection datasets to also check out this data simulator, and the methodologies for credit card fraud detection presented in the book.

This code implements a logistic regression model to detect fraudulent credit card transactions.

Dataset
The code uses the Kaggle Credit Card Fraud Detection dataset, which contains 284,807 transactions made by European cardholders in September 2013. The dataset is highly unbalanced, with only 492 frauds out of 284,807 transactions.

Preprocessing
The code first preprocesses the data by removing the Class column and then randomly sampling 30 fraudulent transactions to balance the dataset.

Training and Evaluation
The code then splits the data into a training set and a test set. The training set is used to fit the logistic regression model, and the test set is used to evaluate the model.

The logistic regression model is fitted using the fit() method. The accuracy of the model is evaluated using the accuracy_score() method.

Results
The logistic regression model achieves an accuracy of 99.3% on the training set and 92.4% on the test set.
