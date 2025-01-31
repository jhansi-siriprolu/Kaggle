# Kaggle
Includes Notebooks worked on Kaggle datasets
## [time-series-analysis-delhi-2.ipynb](https://github.com/jhansi-siriprolu/Kaggle/blob/53e58833ce99a3343a6ae9e8df8a933bfa61cd37/time-series-analysis-delhi-2.ipynb)
Simple Linear regression model built using Delhi climate data. 
* The notebook includes the Exploratory Data Analysis, Data Preprocessing.
* Data is split using Time Series cross validation technique.
* Evaluation Metric: RMSEi is used. RMSLE(L for log) would not be required as there are no much outliers. Mean Absolute percentage /Mean Absolute Scale Error would not be applicable as we are not comparing 2 time series data on same model.
* Finally, Linear regression model is used in predicting the time series.

## [Credit card approval Prediction](https://www.kaggle.com/code/jhansisri/credit-card-approval-prediction/edit#Train-test-split)
XGBClassifier model is used for binary classification of customers.
* EDA Involves the box plots of numeric columns, crosstab of categorical columns and target column.
* Data Preprocessing involved Train test split, One hot encoding categorical columns and MinMaxScaler for numeric columns.
* Basic XGBClassifier is built on this transformed data.
* Performance tuning of the XGBClassifier is done using GridSearchCV on max_depth, learning_rate, colsample_bytree, regularization parameter gamma.
* Evaluation metric of f1_score along with precision and recall scores is considered. As this is a financial sector, False positives would result in loss of business with potential customers & False negatives in money loss, this f1_score is considered as fair metric in this case.
