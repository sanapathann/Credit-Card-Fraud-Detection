# Credit-Card-Fraud-Detection

The dataset for this project was taken from Kaggle.

Link: https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

The dataset contains transactions made by credit cards in September 2013 by European cardholders over 2 days. The dataset consists of  284,807 transactions out of which only 492 are fraudulent.  The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.

It contains only numerical input variables which are the result of a PCA transformation. Unfortunately, due to confidentiality issues, we cannot provide the original features and more background information about the data. Features V1, V2, … V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'. Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset. The feature 'Amount' is the transaction Amount, this feature can be used for example-dependant cost-sensitive learning. Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise. 

We proposed two hybrid machine learning models: 
1. Isolation Forest with XGBoost (IFXGB) and,
2. Local Outlier Factor with Multi-layer perceptron (LOFMLP )

We compare the performances of the hybrid models against baseline XGB and MLP models.
