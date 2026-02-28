# Impact of US Recession on Indian Economy F.Y. 2022-23
### Capstone project analyzing the impact of US GDP recession on Indian GDP growth using Time Series models (ARIMA/SARIMA), Machine Learning (SVR, MLP, Random Forest), and Deep Learning (LSTM), with 5-year economic forecasting.  

---

## Business Problem

Global recessions create ripple effects across emerging markets.  
This project evaluates:

> **How strongly does a US economic downturn impact India's GDP growth?**

The objective was to build an end-to-end forecasting pipeline that:

- Predicts US GDP growth using macroeconomic indicators  
- Quantifies spillover impact on Indian GDP  
- Provides a 5-year forward-looking economic outlook  

---

## Dataset Overview

- **Source:** Federal Reserve Economic Data (FRED)  
- **Frequency:** Quarterly  
- **Period Covered:** 1960 – 2022  
- **Records:** 252  

### Target Variable
- US GDP Growth Rate  

### Exogenous US Variables
- Total Manufacturing Production (TMP)  
- Real Effective Exchange Rate (REER)  
- Unemployment Rate (UR)  
- M3 Money Supply (M3)  
- Total Unit Labor Cost: Manufacturing (TULCM)  
- Consumer Price Index (CPI)  
- Total Share Prices (TSP)  
- Total Construction Production (TC)  

### Indian GDP Data

- **Source:** Federal Reserve Economic Data (FRED)
- **Frequency:** Quarterly (Seasonally Adjusted)
- **Period Covered:** 2012 – 2022
- **Usage:** Dependent variable in regression analysis

Indian GDP Growth Rate was used to:

- Establish a relationship between US GDP and Indian GDP
- Build a Simple Linear Regression model
- Quantify the spillover impact of US recession on India
- Forecast India’s GDP based on predicted US GDP values
---

## Technical Approach

### Data Preparation

- Missing value prediction using ML models  
- Stationarity testing (ADF & KPSS tests)  
- First-order differencing for non-stationary series  
- Feature engineering using 4-quarter lag windows  

---

### Modeling Framework

#### Statistical Models (R)
- ARIMA  
- SARIMA  

#### Machine Learning Models (Python)
- Support Vector Regressor (SVR)  
- Multi-Layer Perceptron (MLP)  
- Decision Tree Regressor  
- **Random Forest Regressor (Best Performing)**  
- Long Short-Term Memory (LSTM)  

---

### Model Evaluation Metrics

Models were compared using:

- MAE (Mean Absolute Error)  
- RMSE (Root Mean Squared Error)  
- MAPE (Mean Absolute Percentage Error)  

A hybrid modeling approach was used to optimize forecasting performance.

---

## Key Results

- Random Forest achieved the lowest MAE  
- Strong positive correlation between US and Indian GDP growth  
- Estimated negative impact of US recession on Indian GDP ≈ **0.02%**  
- Forecast suggests slowdown but no severe contraction  

---

## Business Insights

- The US economy does influence India, but the impact is:
  - Asymmetric  
  - Non-linear  
  - Significantly cushioned  

- India demonstrates structural resilience against US-led downturns.

---
## Project Significance

This project demonstrates:

- Application of econometric and machine learning models to macroeconomic forecasting  
- Handling and transformation of non-stationary time series data  
- Implementation of hybrid modeling techniques combining statistical and ML approaches  
- Cross-country economic impact analysis using regression modeling  

The findings provide practical insights for:

- Policymakers assessing global economic vulnerability  
- Investors evaluating international exposure risk  
- Economic analysts studying recession spillover dynamics  

The modeling framework can be extended to other emerging markets to evaluate global economic interdependencies.

## Tech Stack

**Languages:**  
- Python  
- R  

**Libraries & Tools:**  
- scikit-learn  
- TensorFlow / Keras  
- statsmodels  
- pandas  
- matplotlib  
- forecast (R)  
- tseries (R)  

---
