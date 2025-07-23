# Time Series Econometrics Assignments

## Overview
This repository contains three group assignments from an econometrics course focused on time series analysis. The assignments analyze financial time series data (Bitcoin prices, S&P 500 indices, and Pfizer stock prices) to model mean and volatility, assess stationarity, and evaluate model performance. The work demonstrates proficiency in applying econometric techniques such as ARIMA, GARCH, EGARCH, APARCH, unit root tests, and machine learning, using Python for data analysis and visualization.

## Repository Structure
/data: Input datasets (Data_for_HW1.xlsx, Data HW2.xlsx, PFE data via Yahoo Finance).

/scripts: Python notebooks for each assignment:
- HW1.ipynb: Bitcoin price and log return analysis.
- HW2.ipynb: S&P 500 price and dividend index analysis.
- HW3_Class17_Group11.ipynb: Pfizer (PFE) stock time series modeling and ML forecasting.

## Assignment Details

### Homework 1: Bitcoin Price and Log Returns
Objective: Analyze Bitcoin price index and log returns from November 2020 to December 2024.

Key Tasks:
- Plot correlograms (ACF/PACF) to assess stationarity.
- Compute summary statistics and conduct Jarque-Bera test.
- Fit ARMA and CER models.
- Perform residual diagnostics.

### Homework 2: S&P 500 Price and Dividend Indices
Objective: Analyze S&P 500 price and dividend indices, focusing on stationarity, cointegration, and volatility.

Key Tasks:
- Unit root tests (ADF, PP, KPSS).
- OLS regression and cointegration analysis.
- Model log returns using ARMA and EGARCH.
- Evaluate model performance using BIC and residual tests.

### Homework 3: PFE Stock Time Series and Forecasting
Objective: Model Pfizer (PFE) stock prices and returns to evaluate mean and volatility structures, and compare traditional econometric models to machine learning forecasts.

Key Tasks:
- Conduct visual and statistical stationarity analysis.
- Fit ARMA models for returns and assess model fit.
- Estimate EGARCH and APARCH models for volatility.
- Compare volatility models using AIC and auxiliary regressions.
- Perform out-of-sample forecasts using both econometric and ML models (e.g., XGBoost or Random Forest).
- Evaluate predictive performance using MSFE and visualization.

Key Findings:
- PFE returns are stationary, enabling ARMA modeling.
- EGARCH and APARCH models capture volatility clustering.
- ML models can rival econometric models depending on feature engineering and validation.

## Tools and Technologies
Programming Language: Python

Libraries: pandas, numpy, statsmodels, arch, matplotlib, seaborn, plotly, scipy, openpyxl, yfinance, scikit-learn, xgboost

Environment: Jupyter Notebooks

Data Sources: Provided datasets and Yahoo Finance (PFE stock)

## How to Use

Clone the repository:
bash

git clone https://github.com/Grizozi/time-series-econometrics.git

Install dependencies:
bash

pip install -r requirements.txt

Run the notebooks in /scripts to reproduce the analysis.

Datasets in /data are referenced in the scripts.

## License
This repository is licensed under the MIT License. See the LICENSE file for details.

