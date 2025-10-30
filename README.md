
# ⏳ Time Series Analysis and Forecasting with ARIMA

This project focuses on analyzing and forecasting **Italy’s 2016 total solar generation** and **electricity load** using the **ARIMA (AutoRegressive Integrated Moving Average)** model. The analysis includes data preprocessing, visualization, stationarity testing, model building, and forecasting.

## 📊 Overview

The dataset contains hourly records of electricity **load** and **solar generation** throughout 2016. The project walks through every step of a complete time series analysis pipeline — from cleaning and visualization to modeling and evaluation.

## 🧩 Steps Implemented

1. **Data Loading and Cleaning**

   * Handled missing values using forward fill (`ffill`).
   * Converted `utc_timestamp` to datetime format.

2. **Exploratory Data Analysis**

   * Visualized load and solar generation trends over time.
   * Observed daily and seasonal patterns.

3. **Stationarity Check**

   * Performed the **Augmented Dickey-Fuller (ADF)** test.
   * Both `IT_load_new` and `IT_solar_generation` were found to be stationary.

4. **Model Building (ARIMA)**

   * Determined ARIMA parameters `(p, d, q)` using **ACF** and **PACF** plots.
   * Built ARIMA models and evaluated them on test data (80/20 split).

5. **Model Evaluation**

   * Calculated **Root Mean Squared Error (RMSE)** for model performance.
   * Compared actual vs predicted values visually.

## 📈 Results Summary

| Time Series         | Best ARIMA Order | RMSE   |
| ------------------- | ---------------- | ------ |
| IT_load_new         | (2,0,2)          | ≈ 7715 |
| IT_solar_generation | (2,0,2)          | ≈ 2486 |

Both models captured the general patterns and fluctuations well, with moderate accuracy reflected by the RMSE values.

## 🛠️ Technologies Used

* **Python**
* **Pandas**, **NumPy**
* **Matplotlib**
* **Statsmodels**
* **Scikit-learn**

## 📅 Dataset

**File:** `TimeSeries_TotalSolarGen_and_Load_IT_2016.csv`
Contains hourly electricity load and solar generation data for Italy during 2016.

## 📚 Key Learnings

* How to make time series data stationary for ARIMA modeling.
* How to interpret ACF and PACF plots for parameter tuning.
* How to evaluate and visualize ARIMA model forecasts.

