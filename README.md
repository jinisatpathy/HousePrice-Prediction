# House Price Prediction
The dataset used in this analysis can be obtained from https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data

# Problem Definition
Kaggle have given a dataset and have included all necessary features and wants to have a estimated price of house in Ames, Iowa.

# Dataset
The data is given to predict final price of a house in Ames, Iowa. It presenta a wide range of features hepful in predicting the price. There are two datasets given namely train and test. Test dataset have all features but target i.e SalePrice is excluded.


# Data Preprocessing
Removed suspicious outliers by seeing Target. Also, removed some outliesr which had most suspicious features. Handled Null values differently for different features.

## Target
![Target](https://user-images.githubusercontent.com/46856195/83021979-2cff5880-a06e-11ea-9585-3934fd979353.png)

## Numerical Column
![Numerical](https://user-images.githubusercontent.com/46856195/83022149-6e900380-a06e-11ea-8131-d3df0b1cedf8.png)

## Categorical Column
![Columns](https://user-images.githubusercontent.com/46856195/83021796-e578cc80-a06d-11ea-8932-63be87c19b42.png)

## Null Values
![Null](https://user-images.githubusercontent.com/46856195/83022359-c2025180-a06e-11ea-972a-e07cb9641d4b.png)

Most NULL values shows abscence of features hence filled with 'None'. Mostly filled features with mode values and 0 in numerical columns where the NULL values because of dependent feature. 

## Skew
![Skew](https://user-images.githubusercontent.com/46856195/83023195-ed397080-a06f-11ea-9fd1-9126c35a952e.png)
Used Box-cox transformation.


# Feature Engineering
Created new features such as TotalFloorArea, HouseQuality, TotalBathrooms and TotalPorchArea.

# Model
Tried different models such as Light Gradient Boosting Regressor, XGBoost Regressor,  Ridge Regressor, Support Vector Regressor, Gradient Boosting Regressor, Random Forest Regressor. Also stacked up all regressors and tried to optimise with different models.Used cross-validation RMSE for evaluation

# Prediction
I tried to  blend all model's predictions with different weight and found out the best weight. Blending models makes the final predictions more robust to overfitting. 

![Model](https://user-images.githubusercontent.com/46856195/83023723-a26c2880-a070-11ea-866b-acfd817b5010.png)

RMSE score on train data: 0.04187.RMSE score on test data:  0.12035

