# Housing-Prices
Built a prediction model to predict housing price using The Ames Housing Data Set.
The Data Set has 79 variables, containing numeric and categorical variables, ranging from size of the house to type of ceiling.
Employed Feature engineering techniques, binarization and Pricipal Component Analysis to reduce the dimensionality of the Data set.
Applied Lasso regression, Ridge regression and Elastic Net reguralization on the model and obtained the following Results:

Ridge Regression:
Best alpha : 30.0
The Alpha  required for better precision is centered around 30.
Best alpha : 24.0
Ridge RMSE on Training set : 0.1154057232845079
Ridge RMSE on Test set : 0.11642721377799554

Lasso Regression:
Best alpha : 0.0006
The Alpha  required for better precision is centered around 0.0006
Best alpha : 0.0006
Lasso RMSE on Training set : 0.11411150837458059
Lasso RMSE on Test set : 0.11583213221750702

Elastic Net:
Best l1_ratio : 1.0
Best alpha : 0.0006
The l1_ratio  required for better precision is centered around 1.0
Best l1_ratio : 1.0
Best alpha : 0.0006
The l1_ratio and Alpha  required for better precision is centered around at 1.0 and 0.0006
Best l1_ratio : 1.0
Best alpha : 0.0006
ElasticNet RMSE on Training set : 0.11411150837458059
ElasticNet RMSE on Test set : 0.11583213221750702
