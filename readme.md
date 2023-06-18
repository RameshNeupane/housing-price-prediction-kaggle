# Housing Price Prediction

This repository contains practice code from the course **'Intermediate Machine Learning'** offered by **Kaggle**.

## Data Description
1. [train.csv](https://github.com/RameshNeupane/housing-price-prediction-kaggle/blob/master/train.csv): Training dataset (for training + validation)
2. [test.csv](https://github.com/RameshNeupane/housing-price-prediction-kaggle/blob/master/test.csv): Testing dataset (for prediction)
3. [data_description.txt](https://github.com/RameshNeupane/housing-price-prediction-kaggle/blob/master/data_description.txt): Description of various input data and target i.e. columns with different input categories

## Course Breakdown

### 1. Introduction

- Course Introduction
- Simple Random Forest model
- **[model.ipynb](https://github.com/RameshNeupane/housing-price-prediction-kaggle/blob/master/model.ipynb)**: Practice code
- **[submission.csv](https://github.com/RameshNeupane/housing-price-prediction-kaggle/blob/master/submission.csv)**: Predictions generated for `test.csv` using model from `model.ipynb`

### 2. Missing Values

- Dealing with the missing values
- Three approaches:
  - Drop columns with missing values
  - Imputation
  - Extension to imputation
- Using `SimpleImputation` class from `sklearn.impute`
- **[missing_values.ipynb](https://github.com/RameshNeupane/housing-price-prediction-kaggle/blob/master/missing_values.ipynb)**: Practice code
- **[prediction-missing-values.csv](https://github.com/RameshNeupane/housing-price-prediction-kaggle/blob/master/prediction-missing-value.csv)**: Predictions generated for `test.csv` using model from `missing_values.ipynb`

### 3. Categorical Variables

- Dealing with non-numeric i.e. categorical data
- Three approaches:
  - Drop categorical variables
  - Ordinal encoding
  - One-hot encoding
- Using `OrdinalEncoder` and `OneHotEncoder` classes from `sklearn.preprocessing`
- **[categorical_variables.ipynb](https://github.com/RameshNeupane/housing-price-prediction-kaggle/blob/master/categorical_variables.ipynb)**: Practice code
- **[prediction_categorical_variable.csv](https://github.com/RameshNeupane/housing-price-prediction-kaggle/blob/master/prediction_categorical_variable.csv)**: Predictions generated for `test.csv` using model from `prediction_categorical_variable.ipynb`

### 4. Pipeline

- Simple way to keep data preprocessing and modeling code organized
- Benefits:
  - Cleaner code
  - Fewer bugs
  - Easier to productionize
  - More options for model validation
- Steps:
  - Define preprocessing steps
  - Define model
  - Create and evaluate pipeline
- Using `ColumnTransformer` class from `sklearn.compose` and using `Pipeline` class from `sklearn.pipeline`
- **[pipeline.ipynb](https://github.com/RameshNeupane/housing-price-prediction-kaggle/blob/master/pipeline.ipynb)**: Practice code
- **[pipeline_predictions.csv](https://github.com/RameshNeupane/housing-price-prediction-kaggle/blob/master/pipeline_predictions.csv)**: Predictions generated for `test.csv` using model from `pipeline.ipynb`

### 5. Cross Validation

- Run modeling process on different subsets of the data to get multiple measures of model quality
- Yields a much better measure of model quality
- Good choice for small dataset
- Using `cross_val_score` from `sklearn.model_selection`
- **[cross_validation.ipynb](https://github.com/RameshNeupane/housing-price-prediction-kaggle/blob/master/cross-validation.ipynb)**: Practice code

### 6. XGBoost: Extreme Gradient Boosting

- The most accurate modeling technique for structured data i.e. pd.DataFrame
- Build and optimise model with **gradient boosting**
- Using `XGBRegressor` class from `xgboost`
- Parameter tuning:
  - n_estimator
  - early_stopping_rounds
  - learning_rate
  - n_jobs
- **[XGBoost.ipynb](https://github.com/RameshNeupane/housing-price-prediction-kaggle/blob/master/XGBoost.ipynb)**: Practice code
- **[XGBoost_predictions.csv](https://github.com/RameshNeupane/housing-price-prediction-kaggle/blob/master/XGBoost_predictions.csv)**: Predictions generated for `test.csv` using model from `XGBoost.ipynb`

### 7. Data Leakage

- Data leakage (or leakage) happens when your training data contains information about the target, but similar data will not be available when the model is used for prediction
- Two main type:
  - Target leakage
  - Train-test contamination

## Certificate

[Here](https://github.com/RameshNeupane/kaggle-certificates/blob/master/Ramesh%20Neupane%20-%20Intermediate%20Machine%20Learning.png)
