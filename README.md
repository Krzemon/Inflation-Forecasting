# Inflation Forecasting in Poland using Neural Networks

Predictive model based on neural networks for forecasting **monthly inflation in Poland** using historical macroeconomic indicators published by the Polish Central Statistical Office (GUS).

## Project Overview

The goal of this project is to build machine learning models capable of forecasting **monthly inflation (CPI)** in Poland using historical economic data.

Inflation is one of the most important macroeconomic indicators affecting monetary policy, interest rates, and financial markets. Accurate forecasting can support economic analysis, policy evaluation, and financial decision-making.

The models implemented in this project use historical time series data and neural network architectures to learn patterns in inflation dynamics and generate future predictions.

## Data Source

The dataset used in this project comes from the **Polish Central Statistical Office (GUS)** and includes historical monthly Consumer Price Index (CPI) indicators.

Data source:  
https://stat.gov.pl/obszary-tematyczne/ceny-handel/wskazniki-cen/wskazniki-cen-towarow-i-uslug-konsumpcyjnych-pot-inflacja-/miesieczne-wskazniki-cen-towarow-i-uslug-konsumpcyjnych-od-1982-roku/

The dataset contains monthly CPI values starting from **1982**, allowing the creation of long time series suitable for machine learning and deep learning models. :contentReference[oaicite:0]{index=0}

## Methods

The project implements and compares two neural network approaches for time series forecasting.

### LSTM (Long Short-Term Memory)

LSTM networks are a type of **recurrent neural network (RNN)** designed to capture long-term dependencies in sequential data. They are particularly suitable for time series forecasting because they can learn temporal patterns and trends in economic indicators.

In this project, the LSTM model learns relationships between past inflation values and predicts future monthly CPI values.

### MLP Regression

The **MLPRegressor (Multi-Layer Perceptron)** is a feed-forward neural network used for regression tasks. The model learns nonlinear relationships between lagged inflation values and the target variable.

Compared to LSTM, MLP does not explicitly model temporal dependencies but can still perform well when the time series is transformed into supervised learning format using lag features.

## Workflow

The project workflow consists of the following steps:

1. Data collection from GUS
2. Data preprocessing and cleaning
3. Feature engineering
4. Model training
5. Model evaluation
6. Inflation prediction

## Requirements

Main libraries used in the project:

- Python 3.x
- NumPy
- Pandas
- Sklearn
- TensorFlow
- Matplotlib
