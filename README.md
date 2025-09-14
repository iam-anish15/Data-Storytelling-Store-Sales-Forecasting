# Data Storytelling: Forecasting Future Store Sales with AI 📈

## 📌 Project Overview  
This project is part of my **21 Days, 21 Projects** journey with GeeksforGeeks.  
It focuses on **time series forecasting** using historical airline passenger data. By applying ARIMA and SARIMA models, we predict **future store/airline sales trends** and uncover insights into seasonality and growth patterns.  

We also explore **data decomposition, stationarity testing, and model evaluation** to ensure accurate forecasts and understand the underlying dynamics of the time series.  

---

## 📊 Key Insights from Analysis  

### Time Series Decomposition  
- **Trend**: The number of passengers shows a consistent upward trajectory over time.  
- **Seasonality**: Clear repeating annual patterns observed with peaks and troughs.  
- **Variance**: Seasonal fluctuations increase over time, indicating the need for variance stabilization.

### Stationarity Testing (ADF Test)  
- Original series: ❌ Non-stationary (p-value ≈ 0.99)  
- Log-transformed: ❌ Non-stationary (p-value ≈ 0.42)  
- Log + Differencing: ✅ Stationary (p-value ≈ 0.02)  
- Only after **log transformation + differencing** did the series become stationary, making it suitable for ARIMA/SARIMA modeling.  

### ARIMA vs SARIMA Modeling  
- **ARIMA (non-seasonal)**: Captures overall trend but **misses seasonal peaks**, resulting in higher RMSE.  
- **SARIMA (seasonal)**: Accurately captures **both trend and seasonality**, producing realistic forecasts with lower RMSE.  

---

## 📂 Repository Contents  
- `Predicting_Future_Store_Sales_with_AI.ipynb` → Notebook with complete time series analysis, ARIMA/SARIMA models, and evaluation  
- `airline_passenger_timeseries.csv` → Dataset used for analysis  
- `README.md` → Project documentation  

---

## 🔮 Next Steps  
Planned future enhancements:  
- 📈 Explore **advanced forecasting models** such as Prophet or LSTM for higher accuracy.  
- 🎨 Build **interactive dashboards** with Plotly / Streamlit to visualize forecasts.  
- 🧩 Incorporate additional external factors (e.g., holidays, promotions) to refine predictions.  

---

## 📌 About  
**Projects in 21 Days Batch 1_L6: Data Storytelling: Forecasting Store/Passenger Sales**  
This project applies **time series decomposition + ARIMA/SARIMA modeling** to forecast future sales, demonstrating the importance of trend and seasonality analysis for **data-driven decision-making and storytelling**.  
