# Kaggle
Includes Notebooks worked on Kaggle datasets

## [time-series-analysis-delhi-2.ipynb](https://github.com/jhansi-siriprolu/Kaggle/blob/53e58833ce99a3343a6ae9e8df8a933bfa61cd37/time-series-analysis-delhi-2.ipynb)
Simple Linear regression model built using Delhi climate data.
* The notebook includes the Exploratory Data Analysis, Data Preprocessing.
* Data is split using Time Series cross-validation technique.
* Evaluation Metric: RMSE is used. RMSLE (L for log) would not be required as there are not many outliers. Mean Absolute Percentage / Mean Absolute Scale Error would not be applicable as we are not comparing two time series data on the same model.
* Finally, a Linear Regression model is used in predicting the time series.

## [Credit Card Approval Prediction](https://www.kaggle.com/code/jhansisri/credit-card-approval-prediction/edit#Train-test-split)
XGBClassifier model is used for binary classification of customers.
* EDA involves box plots of numeric columns, and a crosstab of categorical columns and the target column.
* Data Preprocessing involves Train-Test split, One-Hot Encoding of categorical columns, and MinMaxScaler for numeric columns.
* A basic XGBClassifier is built on this transformed data.
* Performance tuning of the XGBClassifier is done using GridSearchCV on max_depth, learning_rate, colsample_bytree, and the regularization parameter gamma.
* The evaluation metric of f1_score along with precision and recall scores is considered. As this is a financial sector, False Positives would result in a loss of business with potential customers & False Negatives in money loss; hence, f1_score is considered a fair metric in this case.

## [GridSearchCV for Hyperparameter Tuning](https://www.kaggle.com/code/jhansisri/binaryclassification-depression)
A Random Forest classifier is optimized using GridSearchCV.
* The dataset undergoes preprocessing, including categorical encoding using LabelEncoder and numerical scaling.
* The model pipeline consists of preprocessing followed by a RandomForestClassifier.
* Hyperparameter tuning is performed using GridSearchCV with cross-validation.
* The best hyperparameters and model performance are evaluated.

## [Keras Binary Classification](https://www.kaggle.com/code/jhansisri/keras-binaryclassification)
A binary classification task implemented using Keras and integrated into a Scikit-Learn pipeline.
* Categorical and numerical features are preprocessed using Ordinal Encoding and Scaling.
* A Sequential Keras model with Dense layers is built for classification.
* The model is trained within a pipeline setup without GridSearchCV.
* The final predictions are generated and prepared for submission.
