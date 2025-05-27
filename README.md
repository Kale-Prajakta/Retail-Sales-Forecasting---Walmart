# Retail Sales Forecasting - Walmart

This project forecasts weekly sales for Walmart stores using regression models and time-based features.

---

## 📦 Dataset
- **Source:** [Kaggle - Walmart Store Sales Forecasting](https://www.kaggle.com/competitions/walmart-recruiting-store-sales-forecasting)
- **Files Used:** `train.csv`, `test.csv`, `features.csv`, `stores.csv`

---

## 🔧 Feature Engineering
- Merged: `train`, `features`, `stores`
- Extracted:
  - `Year`, `Month`, `Week`, `Day`, `DayOfWeek`
  - `IsMonthStart`, `IsMonthEnd`
- Included promotions and markdown features

---

## 📊 Models
### Linear Regression
- Simple baseline model
- **RMSE:** *[e.g., 22,000]*

### XGBoost
- Handles non-linear relationships better
- **RMSE:** *[e.g., 17,500]*

---

## 📉 Visualization
- Plotted predicted vs actual sales
- XGBoost closely follows the actual trend

---

## 📈 Business Insights
- Holidays and markdowns strongly impact sales
- XGBoost helps capture complex seasonality
- Feature importance can inform promotions planning

---

## 🧠 Tools & Libraries
- Python, Pandas, Seaborn, Scikit-learn, XGBoost, Matplotlib
