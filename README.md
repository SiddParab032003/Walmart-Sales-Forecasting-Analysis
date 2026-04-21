![Python](https://img.shields.io/badge/Python-3.12-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-green)
![Time Series](https://img.shields.io/badge/Model-SARIMA-orange)
![Status](https://img.shields.io/badge/Project-Completed-brightgreen)

# Walmart-Sales-Forecasting-Analysis
This project analyzes Walmart sales data and applies time series models (ARIMA &amp; SARIMA) to generate accurate forecasts and business insights.

# 📊 Walmart Sales Forecasting & Analysis

##  Project Overview
This project focuses on analyzing Walmart's weekly sales data to uncover key business insights and forecast future sales using time series models.

The objective is to understand factors affecting sales and build predictive models to assist in inventory management and demand planning.

---

##  Dataset Description
The dataset contains weekly sales data for multiple Walmart stores along with economic and environmental factors:

- Store: Store number
- Date: Week of sales
- Weekly_Sales: Sales for the given store
- Holiday_Flag: Whether the week is a holiday
- Temperature: Temperature during the week
- Fuel_Price: Fuel cost in the region
- CPI: Consumer Price Index
- Unemployment: Unemployment rate

---

##  Exploratory Data Analysis (EDA)

Key analysis performed:

- ✔ Missing value check (no missing data found)
- ✔ Outlier detection using boxplots
- ✔ Correlation analysis

###  Key Insights:
- Unemployment, CPI, and Temperature have **minimal impact** on sales
- Strong **seasonal trend observed**
  - Peak sales in **December**
  - Lowest sales in **January**
- Significant variation in performance across stores

---

##  Top & Worst Performing Stores

- **Top Store:** Store 20 (~2.1M avg weekly sales)
- **Worst Store:** Store 33 (~0.26M avg weekly sales)
- **Difference:** ~1.85M → highlights major performance gap

---

##  Time Series Forecasting

### 🔹 ARIMA Model
- Used for baseline forecasting
- Captures trend but not seasonality
- Produces relatively flat predictions

### 🔹 SARIMA Model (Improved Model)
- Captures both **trend and seasonality**
- More realistic predictions
- Accounts for holiday spikes and demand fluctuations

---

## 📊 Model Comparison

| Metric | ARIMA | SARIMA |
|------|------|--------|
| MAE | 285,216 | **66,137 ✅** |
| Seasonality | ❌ | ✅ |
| Accuracy | Moderate | High |
| Real-world fit | Limited | Strong |

 SARIMA significantly outperforms ARIMA due to its ability to capture seasonal patterns.

---

##  Forecast Results

- Sales expected to:
  - Increase during holiday periods (December)
  - Decline after holidays (January)
- SARIMA provides **dynamic and realistic forecasts**

---

##  Technologies Used

- Python 
- Pandas
- NumPy
- Matplotlib
- Statsmodels (ARIMA, SARIMA)
- Scikit-learn (MAE)

---

##  Key Takeaways

- External factors (CPI, Temperature, Unemployment) have limited impact
- Seasonal trends play a major role in retail sales
- SARIMA is more effective for time-series forecasting with seasonality
- Data-driven insights can improve inventory and demand planning

---

##  Future Improvements

- Implement Prophet model for comparison
- Hyperparameter tuning for SARIMA
- Use deep learning models (LSTM)
- Deploy model using a web app

---

##  Conclusion

This project demonstrates how data analysis and time series forecasting can provide actionable business insights. The SARIMA model proved to be the most effective approach for predicting retail sales due to its ability to capture seasonal patterns.

---

##  Author

**Siddharth Parab**
