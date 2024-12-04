# Predictive Modeling for Sales Forecasting using Decision Tree

## Project Overview

This project involves building a predictive machine learning model to estimate monthly sales (or another target variable) based on various features, including product-related, economic, and demographic data. The goal is to preprocess the data, engineer useful features, and use a **Decision Tree Regressor** to achieve accurate predictions.

The project leverages **Decision Tree Regressor**, a simple but effective machine learning algorithm, and employs feature engineering techniques to improve the model's predictive performance.

## Key Features
- **Data Cleaning and Preprocessing:** 
  - Missing values are imputed with the median for numerical features and the most frequent value for categorical features.
  - Outliers are handled by replacing extreme values with the median.
  - Date features are extracted into new variables such as year, month, day, and day of the week.
- **Feature Engineering:** 
  - New features are derived from date columns, and `days_since_launch` is computed as a useful feature.
  - Numerical features are scaled using **StandardScaler**, and categorical features are encoded using **OneHotEncoder**.
- **Modeling:** 
  - A **Decision Tree Regressor** is used to predict monthly sales based on the prepared data.
- **Model Evaluation:** 
  - The model is evaluated using **Mean Absolute Error (MAE)**, a common metric for regression tasks.
- **Submission File:** 
  - After training, the model is used to predict the target for a test dataset, and the results are saved in a CSV file for submission.

## Project Workflow

1. **Data Preprocessing:**
   - Handle missing data by imputing with the median or most frequent value.
   - Extract useful features from date columns (year, month, day, etc.).
   - Replace outliers with the median value based on interquartile range (IQR).
   
2. **Feature Transformation:**
   - Standardize numerical features using **StandardScaler**.
   - Apply **OneHotEncoder** for encoding categorical variables.

3. **Model Training:**
   - Use **Decision Tree Regressor** to predict monthly sales based on the preprocessed and engineered features.

4. **Evaluation and Results:**
   - Evaluate the model using **Mean Absolute Error (MAE)**.
   - Generate predictions for a test dataset and save the results in a submission file.

## How to Use

### Prerequisites

- Python 3.x
- Required libraries:
  - `pandas`
  - `numpy`
  - `scikit-learn`
  - `matplotlib`

You can install the necessary dependencies by running:

```bash
pip install -r requirements.txt
