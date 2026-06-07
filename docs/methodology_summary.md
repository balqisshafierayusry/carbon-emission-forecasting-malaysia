# Methodology Summary

This project follows a six-stage machine learning pipeline:

1. Dataset Building
2. Data Preprocessing
3. Model Selection
4. Model Training and Optimisation
5. Model Evaluation
6. Forecasting Output and Dashboard Visualisation

## Dataset Building

CO₂ emissions data are obtained from Our World in Data, while GDP, population, and energy-use data are obtained from World Bank Open Data. Selected countries are compiled into a country-year panel dataset.

## Data Preprocessing

Preprocessing includes unit standardisation, log transformation, chronological sorting, and lag-feature engineering. Lag variables are created within each country to avoid cross-country leakage.

## Models

Three models are compared:

- ARIMA
- Random Forest Regressor
- XGBoost Regressor

## Train-Test Split

Training period: 1992–2019  
Testing period: 2020–2022

## Evaluation Metrics

- RMSE
- MAE
- MAPE
- R²

## Scenario Forecasting

Forecasts are generated for 2023–2030 under:

- Business-as-Usual scenario
- Low-Carbon Transition scenario
