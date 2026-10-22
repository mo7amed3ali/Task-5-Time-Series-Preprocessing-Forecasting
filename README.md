# Task 5 — Time Series Preprocessing & Forecasting

## Project Overview

This project focuses on time series preprocessing and weather forecasting using historical daily weather data for Cairo, Egypt, from 2016 to 2025.

The main objective is to analyze daily average temperature patterns, prepare the time series for forecasting, and evaluate statistical forecasting models.

## Dataset

* **Location:** Cairo, Egypt
* **Period:** January 2016 – December 2025
* **Target Variable:** `T2M` (Daily Average Temperature)
* **Data Frequency:** Daily

The dataset includes weather measurements and engineered features used during the analysis.

## Tools & Libraries

* Python
* Pandas and NumPy
* Matplotlib
* Statsmodels
* pmdarima

## Project Workflow

1. Load and inspect the prepared weather dataset.
2. Preprocess and structure the daily time series.
3. Test stationarity using ADF and KPSS tests.
4. Analyze autocorrelation using ACF and PACF.
5. Split the data chronologically into training and testing sets.
6. Build and evaluate ARIMA and SARIMAX forecasting models.
7. Use Fourier features to represent annual seasonality.
8. Compare model performance with a Seasonal Naive baseline.
9. Visualize forecasts and 95% confidence intervals.

## Models Evaluated

* ARIMA
* SARIMAX with Fourier seasonal features
* Seasonal Naive baseline

## Results

The SARIMAX model achieved the following results on the test set:

* **MAE:** 1.6093°C
* **RMSE:** 2.1624°C

The Seasonal Naive baseline achieved:

* **MAE:** 2.2851°C
* **RMSE:** 2.9134°C

Based on these metrics, SARIMAX outperformed the Seasonal Naive baseline on this test period.

## Repository Contents

* `Task_5_Time_Series_Preprocessing_Forecasting.ipynb` — Notebook containing preprocessing, statistical analysis, model training, evaluation, and forecasting.
* `cairo_weather_prepared.csv` — Prepared daily weather dataset used in the analysis.

## How to Run

1. Clone or download this repository.
2. Install the required Python libraries.
3. Open the Jupyter Notebook.
4. Run the cells sequentially.

## Limitations

Forecast accuracy depends on historical patterns and the selected model. Forecasts may not capture unexpected weather events or sudden changes.

## Author

Mohamed Ali
