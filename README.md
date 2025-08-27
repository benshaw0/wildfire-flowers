# wildfire-flowers

## Dataset

### Target Variables

*Dataset contains 2555 days (≈7 years) of stem output data*

- **Roses** – Daily Output
- **Hypericum** – Daily Output

### Features

*Dataset contains 1109 days (≈3 years) of weather data*

- **Temperature**
  `[AvgTemp, Temp-1, Temp-2, OutTemp-Avg, OutTemp-Min, OutTemp-Max]`

- **Humidity**
  `[Avg-Hum, Hum-1, Hum-2, OutHum-Avg, OutHum-Min, OutHum-Max]`

- **Wind**
  `[WindSpd-Avg, WindSpd-Max, WindDir-Avg]`

- **Rain**
  `[RainStatus, DailyRain, RainFlow]`

- **Radiation**
  `[Rad-Avg, Rad-Sum]`

- **EC & pH**
  `[EC-Sen, PH-Sen]`

---

## Predictive Modelling

**Problem:** *Multivariate, supervised time series (dependent on both their own history and multiple external/environmental drivers)*

**Objective:** *Predict future stem outputs for a chosen forecast horizon*

### 1. Time Series Modelling
- **SARIMAX** (Seasonal ARIMA with Exogenous Variables)

### 2. Machine Learning (Non-Sequential)
- **Random Forest / Gradient Boosting**

### 3. Deep Learning (Sequential)
- **RNNs – Long Short-Term Memory (LSTM)**

---

## Deployment

**Streamlit dashboard** with the following functionality:

- Upload updated weather forecasts
- Generate yield predictions for roses & hypericum (at defined forecast horizon)
- Visualise predictions with confidence intervals

**Integration with Power BI dashboard** for centralised analysis
