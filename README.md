# ☕ Coffee Shop Demand Forecasting

Forecasting daily customer demand is critical for coffee shops to optimize staffing, manage inventory, and minimize waste.  
This project builds and compares multiple forecasting models to predict daily sales (in cups sold) using historical transaction data.

---

## 📌 Project Goals

- Forecast next 7 days of customer demand
- Evaluate both statistical and ML-based forecasting approaches
- Recommend the most accurate model for operational use

---

## 🧠 Models Built & Evaluated

- ARIMA
- SARIMAX ✅ *(Best performer with MAE ≈ 3.3 cups/day)*
- Auto ARIMA
- Auto SARIMAX
- Custom Auto ARIMA
- LightGBM Regressor

**Metric Used:**  
- Mean Absolute Error (MAE)

---

## 📊 Final Results

![MAE Comparison](./plots/model_mae_comparison.png)

> SARIMAX achieved the lowest forecasting error, making it the recommended model for short-term demand prediction.

---

## 🛠 Features & Pipeline

- Aggregated raw sales into daily time series
- Filled missing dates to create a complete sequence
- Visualized trends and compared forecast curves
- Benchmarked 6 models on the same train/test split

---
## 🛒 Tools & Libraries

- `pandas`, `numpy`, `seaborn`, `matplotlib`
- `statsmodels`, `pmdarima`
- `scikit-learn`, `lightgbm`

---

## 🚀 Future Improvements

- Add external features (e.g., weather, promotions)
- Deploy best model using Streamlit
- Automate daily forecast updates

---
