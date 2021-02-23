# Classification-5-ways
5 strategies to detect fraud from a dataset.


Using the data from https://www.kaggle.com/mlg-ulb/creditcardfraud it is possible to develop machine learning algoritms to predict if a given user is fraudulent or not. In this project 5 attempts are made, Logistic Regression, K-Nearest Neighbour, Support Vector Classifier, Decision Tree Classifier and XGBoost gradient boosting. A brief explanation of every algoritm is made, as well as performace analisys.

The dataset is too big for uploading here, but a smaller balanced sample is avaliable in 'Balanced_data.csv' as well as a 'balancing_data.ipynb' code that build this sample. Some notes about the performace metrics are in the 'Classification 5 ways.ipynb' file

About the data as written in the link:
  "The datasets contains transactions made by credit cards in September 2013 by european cardholders.
This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.

It contains only numerical input variables which are the result of a PCA transformation. Unfortunately, due to confidentiality issues, we cannot provide the original features and more background information about the data. Features V1, V2, … V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'. Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset. The feature 'Amount' is the transaction Amount, this feature can be used for example-dependant cost-senstive learning. Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise."

But what is a PCA transformation?
  Principal Component Analysis is an orthogonal linear transformation that acts in the original data and gives us "new data" in a new coordinate sistem in wich every vector of the basis(our columns) are now orthogonal. With this transformation 






Here are more details on how the models work:

  1-Logistic Regression
  
  
  
  
  
  2-K-Nearest Neighbors
  
  
  
  
  
  3-Support Vector Classifier
  
  
  
  
  
  4-Decision Tree Classifier
  
  
  
  
  
  5-XGBoost
  
  
  
  










