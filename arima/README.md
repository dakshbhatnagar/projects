# Understanding ARIMA and ARMA Models

## Introduction

This project aims to provide a comprehensive understanding of ARIMA (AutoRegressive Integrated Moving Average) and ARMA (AutoRegressive Moving Average) models. These models are pivotal in time series analysis, allowing us to understand and predict future values based on past data.

---

## Table of Contents

1. [Overview](#overview)
2. [Prerequisites](#prerequisites)
3. [ARMA Model](#arma-model)
    - [Autoregressive (AR) Part](#autoregressive-ar-part)
    - [Moving Average (MA) Part](#moving-average-ma-part)
4. [ARIMA Model](#arima-model)
    - [Integrated (I) Part](#integrated-i-part)
5. [Model Building Process](#model-building-process)
6. [Implementation](#implementation)
    - [Data Preparation](#data-preparation)
    - [Parameter Selection](#parameter-selection)
    - [Model Training and Evaluation](#model-training-and-evaluation)
7. [Conclusion](#conclusion)
8. [References](#references)

---

## Overview

Time series forecasting is essential for numerous fields, including finance, economics, and weather forecasting. ARMA and ARIMA models are two of the most commonly used statistical models for analyzing and predicting time series data.

---

## Prerequisites

Before diving into ARIMA and ARMA models, it is recommended to have a basic understanding of:

- Time Series Data
- Statistical concepts (mean, variance, autocorrelation)
- Python programming
    - Libraries: `pandas`, `numpy`, `statsmodels`, `matplotlib`

---

## ARMA Model

### Autoregressive (AR) Part

The AR part of the model involves regressing the variable on its own lagged (past) values. The order of the AR part is denoted by `p`.

**Formula:**
$X_t = c + \sum_{i=1}^{p} \phi_i X_{t-i} + \epsilon_t $

### Moving Average (MA) Part

The MA part involves modeling the error term as a linear combination of error terms occurring contemporaneously and at various times in the past. The order of the MA part is denoted by `q`.

**Formula:**
$ X_t = \mu + \sum_{i=1}^{q} \theta_i \epsilon_{t-i} + \epsilon_t $


---
## ARIMA Model

The ARIMA model is an extension of the ARMA model that includes a differencing step to make the time series stationary. The ARIMA model is denoted by ARIMA(p, d, q) where:

- `p`: order of the autoregressive part
- `d`: degree of differencing
- `q`: order of the moving average part

### Integrated (I) Part

The integrated part refers to the differencing of raw observations to allow for the time series to become stationary. Differencing is a method of transforming a non-stationary series into a stationary one.

---

## Model Building Process

1. **Data Preparation:** Ensure your data is in a proper time series format.
2. **Stationarity Check:** Check if the time series is stationary using methods like the Augmented Dickey-Fuller test.
3. **Parameter Selection:** Use methods like ACF (Autocorrelation Function) and PACF (Partial Autocorrelation Function) plots to identify the values of `p`, `d`, and `q`.
4. **Model Training:** Fit the ARIMA model to the data.
5. **Model Evaluation:** Evaluate the model using metrics like AIC, BIC, and residual diagnostics.

----
## Conclusion

Understanding ARIMA and ARMA models is crucial for time series analysis. These models help in making accurate predictions by capturing the underlying patterns in the data.

---

## References

1. Hyndman, R. J., & Athanasopoulos, G. (2018). Forecasting: principles and practice. OTexts.
2. Box, G. E. P., Jenkins, G. M., Reinsel, G. C., & Ljung, G. M. (2015). Time Series Analysis: Forecasting and Control. Wiley.
3. [Statsmodels Documentation](https://www.statsmodels.org/)
4. [ARIMA Model - Wikipedia](https://en.wikipedia.org/wiki/Autoregressive_integrated_moving_average)

