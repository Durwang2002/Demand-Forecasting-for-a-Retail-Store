# 📊 Retail Demand Forecasting using Time Series Analysis (SARIMA)

A complete time series forecasting project that analyzes daily retail sales data to predict future product demand. This solution helps retail businesses better manage inventory, reduce stockouts, and optimize sales using statistical modeling techniques like SARIMA.

---

## 🚀 Project Overview

Retail businesses face challenges in predicting future product demand due to seasonality, trends, and volatility in sales. This project tackles that challenge by:

- Aggregating and cleaning historical sales data
- Performing stationarity checks using the ADF Test
- Decomposing seasonal trends using STL decomposition
- Building and training a SARIMA (Seasonal ARIMA) model
- Forecasting the next 30 days of sales
- Visualizing trends, forecasts, and confidence intervals

---

## 🛠️ Technologies & Tools Used

| Category | Tools/Tech |
|---------|------------|
| Language | Python 3.x |
| Data Manipulation | Pandas, NumPy |
| Visualization | Matplotlib |
| Time Series | Statsmodels (SARIMA, ADF Test, STL decomposition) |
| Evaluation | Scikit-learn (RMSE) |
| Notebook | Jupyter Notebook / Google Colab |
| Dataset Format | CSV |

---

## 📂 Dataset

The project uses a CSV file named `retail_store_inventory.csv` which includes:

- `Date` (in YYYY-MM-DD format)
- `Units Sold` (numeric count)
- Additional metadata like product category, region (optional)

> You may use synthetic or real sales data, but ensure it includes daily-level sales for accurate time series modeling.

---

## 📈 Forecasting Model

We use the **SARIMA model**: Seasonal Auto-Regressive Integrated Moving Average.
- SARIMA accounts for seasonality and trends over time.
- It uses orders: `(p,d,q)x(P,D,Q,s)` where `s` is the seasonal period (e.g. weekly).

---

## ✅ Project Workflow

### 📌 STEP 1: Install Dependencies

```bash
pip install pandas numpy matplotlib statsmodels scikit-learn
