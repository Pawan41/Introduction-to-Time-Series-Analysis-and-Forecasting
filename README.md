# 📈 Time Series Analysis and Forecasting

## 📌 Overview
This project demonstrates the fundamentals of **Time Series Analysis and Forecasting** using Python. It covers preprocessing, visualization, decomposition, stationarity testing, smoothing techniques, forecasting models, and model evaluation methods.

The project uses real-world stock market data and applies statistical methods to identify trends, seasonality, and patterns for forecasting future values.

---

# 🚀 Features

- Time series data visualization
- Classical decomposition
- STL decomposition
- Stationarity analysis
- Forecasting models implementation
- Smoothing techniques
- Correlation analysis using ACF & PACF
- Model evaluation metrics
- Data preprocessing techniques

---

# 📚 Topics Covered

## 1. Introduction to Time Series
- Definition of time series data
- Real-world applications
- Characteristics of time series
- Goals of time series analysis

## 2. Time Series Decomposition
- Trend
- Seasonality
- Cyclic patterns
- Residuals
- Additive decomposition
- Multiplicative decomposition
- STL decomposition

## 3. Stationarity
- Strict stationarity
- Weak stationarity
- ADF Test
- KPSS Test
- Differencing
- Data transformation
- De-trending
- Seasonal adjustment

## 4. White Noise & Random Walk
- Characteristics
- Identification methods

## 5. Forecasting Models
- AR
- MA
- ARMA
- ARIMA
- SARIMA
- VAR
- VARMA
- VARIMA

## 6. Smoothing Techniques
- Simple Moving Average (SMA)
- Weighted Moving Average (WMA)
- Exponential Moving Average (EMA)
- Exponential Smoothing
- Holt’s Linear Method
- Holt-Winters Method

## 7. Correlation Analysis
- ACF (Autocorrelation Function)
- PACF (Partial Autocorrelation Function)
- Granger Causality Test

## 8. Evaluation Metrics
- MAE
- MSE
- RMSE
- MAPE
- AIC
- BIC

## 9. Data Preprocessing
- Handling missing values
- Handling outliers
- Resampling
- Making data stationary

---

# 🛠️ Technologies Used

- Python
- Pandas
- Matplotlib
- Statsmodels
- yFinance
- Jupyter Notebook

---

# 📦 Installation

Clone the repository:

```bash
git clone https://github.com/Pawan41/Introduction-to-Time-Series-Analysis-and-Forecasting
cd time-series-analysis
```

Install dependencies:

```bash
pip install yfinance pandas matplotlib statsmodels
```

---

# ▶️ Example Usage

## Download Stock Data

```python
import yfinance as yf

stock_data = yf.download('AAPL', start='2024-01-01')
print(stock_data.head())
```

## Classical Decomposition

```python
from statsmodels.tsa.seasonal import seasonal_decompose

decomposition = seasonal_decompose(
    stock_data['Close'],
    model='additive',
    period=30
)
```

## STL Decomposition

```python
from statsmodels.tsa.seasonal import STL

stl = STL(stock_data['Close'], period=30)
result = stl.fit()
```

---

# 📊 Learning Outcomes

By completing this project, you will learn:

- Fundamentals of time series analysis
- Data preprocessing techniques
- Time series decomposition
- Stationarity testing
- Forecasting model implementation
- Smoothing methods
- Forecast evaluation techniques

---

# 🎯 Conclusion

This project provides a complete introduction to time series analysis and forecasting using statistical and machine learning concepts. It combines theoretical understanding with practical implementation to analyze and forecast real-world time-dependent data effectively.

---

# 👨‍💻 Author

Pawan Kumar
