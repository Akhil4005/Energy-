# Energy Consumption Time Series Forecasting

This project focuses on forecasting energy consumption for the upcoming month based on a single month's data. Multiple models were experimented with, and their results were visualized to determine the most accurate forecasting technique.

## Project Overview

The main goal is to predict overall monthly energy consumption. While individual daily predictions may not seem perfectly accurate, the cumulative monthly predictions (sum of predictions across the month) provide more accurate results. The accuracy is measured using a simple metric:

**Percent Error = ( |Experimental Value – Theoretical Value| ÷ Theoretical Value) x 100**

![Energy Consumption Forecasting](images/energy_forecast.png)

> **Note:** Data cleaning and preprocessing for missing values is required. Refer to Jason Brownlee’s [machinelearningmastery blog](https://machinelearningmastery.com/how-to-develop-an-autoregression-forecast-model-for-household-electricity-consumption/) for assistance.

## Methodology

Here are the forecasting methods applied in this project:

1. **ARIMA (AutoRegressive Integrated Moving Average):**
   - Forecasts for one timestep and for the entire month.
   
2. **Facebook Prophet:**
   - Forecasts based on varying amounts of training data.
   
3. **Auto Regression (AR) with Walk-Forward Validation:**
   - Utilizes autoregression with walk-forward validation.
   
4. **Moving Average (MA) with Anomaly Detection:**
   - Implements moving averages and detects anomalies within the data.
   
5. **Deep Learning for Time Series Forecasting:**
   - A neural network model is used for time series prediction.

## Results

The overall monthly energy consumption prediction is compared to the actual values using the percent error metric mentioned above. Detailed experimental results, including plots for each method, are available in the Jupyter notebook.

### Sample ARIMA Prediction Plot:

![ARIMA Prediction](images/arima_plot.png)

## Installation & Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/AkhilKumar/your-repo.git
