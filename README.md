# Time Series Forecasting of India’s Month-over-Month Inflation

This project explores the behavior and forecasting of India’s monthly inflation rates from 1959 to 2022 using classical time series decomposition and multiple model-fitting techniques. It was completed as part of a university project with a team of 6 students from the Department of Statistics, Kirori Mal College (University of Delhi).

---

## 🎯 Objectives

- Decompose inflation data into trend, seasonal, cyclical, and random components
- Test for stationarity using the Augmented Dickey-Fuller test
- Fit various time series models (Simple Seasonal, SARIMA, ARIMA)
- Evaluate and compare models based on error metrics and predictive intervals
- Forecast future inflation values and identify macroeconomic patterns

---

## 🔍 Highlights of the Analysis

- **Data Period**: Monthly data from 1959 to 2022  
- **Decomposition**: Multiplicative time series model  
- **Stationarity**: Confirmed via ADF Test (p-value < 0.01)  
- **Cyclical Analysis**: Harmonic analysis used to detect oscillations (19th lambda significant)  
- **Model Comparison**:

| Model | Stationary R² | RMSE | MAE | BIC | Prediction Interval Width |
|-------|----------------|------|-----|-----|----------------------------|
| Simple Seasonal | 0.641 | 0.749 | 0.554 | -0.562 | 2.939 |
| SARIMA(0,0,2)(1,0,1)[12] | 0.378 | 0.767 | 0.560 | -0.488 | 3.650 |
| ARIMA(3,0,4) | 0.337 | 0.793 | 0.586 | -0.394 | 3.767 |

- **Best Fit**: Simple Seasonal model based on lowest RMSE and narrowest forecast interval  
- **Conclusion**: Data showed strong yearly seasonality and low trend over decades. Structural shocks (oil crisis, economic liberalization, demonetization, COVID-19) were visible in data movements.

---

## 📈 Methods Used

- Time Series Decomposition (Trend, Seasonal, Cyclical, Random)
- ADF Test for Stationarity
- Auto-correlation & Partial Autocorrelation (ACF, PACF)
- ARIMA and SARIMA model fitting
- Model evaluation using R², RMSE, MAE, BIC
- Forecasting using Simple Seasonal and SARIMA models

---

## 🛠️ Tools & Libraries

- R (TSA, forecast, tseries)
- MS Excel (initial data cleaning & visualization)
- Manual statistical derivations (trend fitting, harmonic analysis)

---

## 🧾 Files Included

| File | Description |
|------|-------------|
| `TSA_Project_Report.pdf` | Final project report including all plots, model results, and interpretation |
| `tsa_model_comparison.xlsx` | Model error metrics and plots (optional) |
| `inflation_data.csv` | Monthly inflation data used for analysis |
| `tsa_script.R` | R script for model fitting and diagnostics (optional) |

---

## 👨‍💻 Contributors

- Dhruv Goel  
- Pratham Singh, Gargi Ghorai, Upali Bera, Samridhi, Goutam Tapperyal  
- Guided by: Dept. of Statistics, Kirori Mal College

---

## 📚 References

- https://www.inflationtool.com/rates/india/historical  
- https://scripbox.com/blog/history-of-inflation-in-india  
- Box-Jenkins Time Series Forecasting Methods  

---
