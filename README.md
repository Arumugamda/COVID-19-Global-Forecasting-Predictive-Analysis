# COVID-19-Global-Forecasting-Predictive-Analysis
## COVID-19 Global Forecasting: Predictive Analysis
This repository contains a comprehensive predictive analysis project focused on forecasting COVID-19 confirmed cases and fatalities globally. The project utilizes time-series modeling techniques, specifically the ARIMA (AutoRegressive Integrated Moving Average) model, to predict future trends based on historical data.

## 📊 Project Overview
The notebook implements a full machine learning pipeline for time-series forecasting, including:
1.Data Acquisition: Loading global COVID-19 datasets (training and testing sets).
2.Exploratory Data Analysis (EDA):Identifying top-impacted countries by confirmed cases (e.g., US, Russia, UK, Spain).Visualizing trends using interactive Plotly bar charts and geographic maps.
3.Statistical Analysis:Performing the Augmented Dickey-Fuller (ADF) test to check for data stationarity.Analyzing Autocorrelation (ACF) and Partial Autocorrelation (PACF) plots to determine model parameters.
4.Time-Series Modeling: Training ARIMA models for various country-region segments to forecast future infection and mortality rates.
5.Forecasting: Generating predictions for a specific timeframe (e.g., starting May 2020).

## 🛠️ Requirements and Installation
To run this notebook, the following Python libraries are required:
>pandas & numpy (Data manipulation)
>>matplotlib, seaborn, & plotly (Visualization)
>>>statsmodels (ARIMA modeling and statistical tests)
>>>scikit-learn (Modeling utilities)You can install the dependencies using:
Bash  pip install pandas numpy matplotlib seaborn plotly statsmodels scikit-learn
## 📈 Methodology
>>>Stationarity Check: The project uses the adfuller test to ensure the time series is stationary before applying ARIMA.
>>>Parameter Selection: ACF and PACF plots are utilized to find the optimal values for the $(p, d, q)$ parameters in the ARIMA model.
>>>Segmented Forecasting: The analysis is performed at a granular level, grouping data by Country_Region and Province_State to provide localized forecasts.
## 📂 Data Description
>>>The analysis relies on two primary CSV files:
    train.csv: Historical daily data including ConfirmedCases and Fatalities for various regions.
    test.csv: The target dates for which the model generates forecasts.
## 🚀 Usage
1.Clone the repository.
2.Ensure train.csv and test.csv are in the project directory.
3.Open predictivefinal.ipynb in Jupyter Notebook or Google Colab.
4.Run all cells to view the EDA, statistical tests, and generated forecasts.
