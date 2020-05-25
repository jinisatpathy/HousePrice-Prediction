# House Price Prediction
The dataset used in this analysis can be obtained from https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data

# Problem Definition
Kaggle have given a dataset and have included all necessary features and wants to have a estimated price of house in Ames, Iowa.

# Dataset
The data is given to predict final price of a house in Ames, Iowa. It presenta a wide range of features hepful in predicting the price. There are two datasets given namely train and test. Test dataset have all features but target i.e SalePrice is excluded.

# Data Preprocessing
Removed suspicious outliers by seeing Target. Also, removed some outliesr which had most suspicious features. Handled Null values differently for different features.

# Feature Engineering
Created new features such as TotalFloorArea, HouseQuality, TotalBathrooms and TotalPorchArea.

# Model
Tried different models such as Light Gradient Boosting Regressor, XGBoost Regressor,  Ridge Regressor, Support Vector Regressor, Gradient Boosting Regressor, Random Forest Regressor. Also stacked up all regressors and tried to optimise with different models. I found out XGboost was best. Then, I tried to  blend all model's predictions with different weight and found out the best weight. Blending models makes the final predictions more robust to overfitting. The RMSE score on train data is 0.06785462793146341.
