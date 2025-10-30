# Energy-Demand-Forecasting
Time-Series Forecasting Using ARIMA
This project focuses on analyzing and forecasting Italy’s 2016 total solar generation and electricity load using the ARIMA (AutoRegressive Integrated Moving Average) model.

📊 Project Overview

The dataset contains hourly records of electricity load and solar generation throughout 2016. The project walks through:

Data preprocessing and handling missing values

Time series visualization

Stationarity testing using the Augmented Dickey-Fuller (ADF) test

Identification of ARIMA parameters (p, d, q) using ACF and PACF plots

Model fitting and prediction for both series

Model performance evaluation using Root Mean Squared Error (RMSE)

Visualization of actual vs predicted values

🧩 Steps Implemented

Data Loading and Cleaning

Handle missing values using forward-fill.

Convert timestamps to datetime objects.

Exploratory Data Analysis

Visualize load and solar generation trends over time.

Identify daily and seasonal patterns.

Stationarity Check

Apply the Augmented Dickey-Fuller test to confirm stationarity.

Model Building

Determine ARIMA parameters via ACF and PACF plots.

Fit ARIMA models with multiple parameter combinations.

Model Evaluation

Compute RMSE to assess prediction accuracy.

Plot actual vs predicted values for comparison.

📈 Results Summary
Time Series	Best ARIMA Order	RMSE
IT_load_new	(2,0,2)	≈ 7715
IT_solar_generation	(2,0,2)	≈ 2486
