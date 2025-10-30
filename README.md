This project focuses on analyzing and forecasting Italy’s 2016 total solar generation and electricity load using the ARIMA (AutoRegressive Integrated Moving Average) model. The analysis includes data preprocessing, visualization, stationarity testing, model building, and forecasting.

📊 Overview

The dataset contains hourly records of electricity load and solar generation throughout 2016. The project walks through every step of a complete time series analysis pipeline — from cleaning and visualization to modeling and evaluation.

🧩 Steps Implemented

Data Loading and Cleaning

Handled missing values using forward fill (ffill).

Converted utc_timestamp to datetime format.

Exploratory Data Analysis

Visualized load and solar generation trends over time.

Observed daily and seasonal patterns.

Stationarity Check

Performed the Augmented Dickey-Fuller (ADF) test.

Both IT_load_new and IT_solar_generation were found to be stationary.

Model Building (ARIMA)

Determined ARIMA parameters (p, d, q) using ACF and PACF plots.

Built ARIMA models and evaluated them on test data (80/20 split).

Model Evaluation

Calculated Root Mean Squared Error (RMSE) for model performance.

Compared actual vs predicted values visually.

📈 Results Summary
Time Series	Best ARIMA Order	RMSE
IT_load_new	(2,0,2)	≈ 7715
IT_solar_generation	(2,0,2)	≈ 2486
