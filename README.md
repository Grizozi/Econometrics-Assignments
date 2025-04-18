# Time Series Econometrics Assignments
## Overview
This repository contains two group assignments from an econometrics course focused on time series analysis. The assignments analyze financial time series data (Bitcoin prices and S&P 500 indices) to model mean and volatility, assess stationarity, and evaluate model performance. The work demonstrates proficiency in applying econometric techniques such as ARIMA, GARCH, and unit root tests, using Python for data analysis and visualization.
## Repository Structure
/data: Input datasets (Data_for_HW1.xlsx, Data HW2.xlsx) containing Bitcoin prices and S&P 500 price/dividend indices.

/scripts: Python scripts or Jupyter notebooks for each assignment:
Econometrics_Group_Homework_1.ipynb: Bitcoin price and log return analysis.

Econometrics_Group_Homework_2.ipynb: S&P 500 price and dividend index analysis.

/results: Output files, including plots (e.g., correlograms, volatility forecasts) and summary tables.

/docs: Assignment descriptions or reports (if available).

## Assignment Details
### Homework 1: Bitcoin Price and Log Returns
Objective: Analyze Bitcoin price index and log returns from November 2020 to December 2024.

Tasks:
Plot correlograms (ACF/PACF) to assess stationarity of Bitcoin prices (non-stationary) and log returns (stationary).

Compute summary statistics and histograms, confirming non-normality of log returns (Jarque-Bera test).

Model log returns using Constant Expected Return (CER) and ARMA models, finding CER as the best fit (lowest AIC/BIC).

Analyze residuals, confirming white noise behavior but non-normal distribution.

Key Findings:
Bitcoin prices exhibit random walk behavior, requiring log return transformation for stationarity.

Log returns resemble a white noise process with no significant autocorrelation.

Non-normality suggests potential for GARCH modeling in future analyses.

### Homework 2: S&P 500 Price and Dividend Indices
Objective: Analyze S&P 500 price and dividend indices, focusing on stationarity, cointegration, and volatility.

Tasks:
Conduct unit root tests (ADF, PP, KPSS) on price and dividend indices, confirming both are I(1).

Perform OLS regression of price on dividend index, detecting cointegration despite residual autocorrelation.

Model S&P 500 log returns using ARMA(0,1) and EGARCH(1,1)/EGARCH(2,2) for volatility clustering.

Evaluate model performance using residual analysis and information criteria (BIC).

Key Findings:
Price and dividend indices are non-stationary but cointegrated, indicating a long-run relationship.

Log returns exhibit volatility clustering and leptokurticity, well-captured by EGARCH(2,2), which outperforms EGARCH(1,1).

EGARCH(2,2) provides an unbiased and efficient predictor of variance (F-test p-value: 0.833).

## Tools and Technologies
Programming Language: Python

Libraries: pandas, numpy, statsmodels, arch, matplotlib, seaborn, plotly, scipy

Environment: Jupyter Notebooks

Data Sources: Provided datasets (Bitcoin prices, S&P 500 indices)

## How to Use
Clone the repository:
bash

git clone https://github.com/Grizozi/time-series-econometrics.git

Install dependencies:
bash

pip install -r requirements.txt

(Create a requirements.txt with: pandas, numpy, statsmodels, arch, matplotlib, seaborn, plotly, scipy, openpyxl.)

Run the notebooks in /scripts to reproduce the analysis.

Datasets in /data are referenced in the scripts.

## License
This repository is licensed under the MIT License. See the LICENSE file for details.

