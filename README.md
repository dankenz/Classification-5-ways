# Classification-5-ways
5 strategies to detect fraud from a dataset.


Using the data from https://www.kaggle.com/mlg-ulb/creditcardfraud it is possible to develop machine learning algoritms to predict if a given user is fraudulent or not. In this project 5 attempts are made, Logistic Regression, K-Nearest Neighbour, Support Vector Classifier, Decision Tree Classifier and XGBoost gradient boosting. A brief explanation of every algoritm is made, as well as performace analisys.

The dataset is too big for uploading here, but a smaller balanced sample is avaliable in 'Balanced_data.csv' as well as a 'balancing_data.ipynb' code that build this sample. Some notes about the performace metrics are in the 'Classification 5 ways.ipynb' file

About the data as written in the link:
  "The datasets contains transactions made by credit cards in September 2013 by european cardholders.
This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.

It contains only numerical input variables which are the result of a PCA transformation. Unfortunately, due to confidentiality issues, we cannot provide the original features and more background information about the data. Features V1, V2, … V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'. Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset. The feature 'Amount' is the transaction Amount, this feature can be used for example-dependant cost-senstive learning. Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise."

But what is a PCA transformation?
  Principal Component Analysis is an orthogonal linear transformation that acts in the original data and gives us "new data" in a new coordinate sistem in wich every vector of the basis(our columns) are now orthogonal.

Here are brief details on how the models work:

  1- Classification by logistic regression tries to fit the data into a sigmoid function. We then use this function to predict if a given row is fraudulent
  
  
  2-K-Nearest Neighbors
  This classification makes a "majority voting" based in the nearest neighbors. The neighbors are defined using some distance metric. A new data that is "near" fraudulent cases is then classified as fraudulent.
  
    
  3-Support Vector Classifier
  Here we look for a hyperplane (or set of) that separates the data by our classifications. We then see where a new data is relative to this set of hyperplanes to predict if it is fraudulent. 
  
  4-Decision Tree Classifier
  A combination of 3 components: nodes,edges and leaf nodes. Nodes are the decisions over features (is v1>0? for exemple), edges are the answers for these questions + the connection to the next node, and leaf nodes are the outcome of the method (fraud or not).
  The algoritm find the best way to build this tree and by inputing new data we can predict the frauds.
  
  
  5-XGBoost
  XGBoost is actually a library that helps in building gradient boosting algoritms. Gradient boosting works by combining weak "learners" into a stronger one. It is common to use decision trees as the weak learners to make this model, so we can expect better performace from this one.
  
  
  
  










