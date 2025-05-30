# Retail Sales Forecasting - Walmart Stores

## Problem Statement
Predict future weekly sales for different Walmart stores using historical data. The aim is to help the business optimize inventory and plan promotions effectively.

## Dataset
Sourced from Kaggle: [Walmart Store Sales Forecasting](https://www.kaggle.com/competitions/walmart-recruiting-store-sales-forecasting)

- `trainw.csv`: Historical sales data  
- `testw.csv`: Test data for prediction  
- `features.csv`: Includes additional features such as markdowns and temperature  
- `stores.csv`: Store-type and size information  

## Approach

### 1. Data Preprocessing
- Merged `train`, `test`, `features`, and `stores` on relevant keys
- Converted `Date` to datetime format

### 2. Feature Engineering
Extracted additional time-based features:
- Year, Month, Week, Day, Day of Week
- IsMonthStart, IsMonthEnd

Promotions & holidays:
- Used `IsHoliday` and `MarkDown` features to model promotional impact

### 3. Models Used
- **Linear Regression**
- **XGBoost Regressor**

### 4. Evaluation Metric
- RMSE (Root Mean Squared Error)
- RMSE (Linear Regression): _reported in notebook_
- RMSE (XGBoost): _reported in notebook_

### 5. Visualization
- Plotted Predicted vs Actual sales using XGBoost (first 100 samples)

## Future Improvements
- Hyperparameter tuning for better XGBoost performance
- Incorporate lag features or rolling averages
- Improve business insights with dollar impact analysis






