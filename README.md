# Carbon Emission Forecasting in Malaysia Using Machine Learning

Final Year Project 2 (FYP 2) project by **Nur Balqis Shafiera Binti Yusry**  
Bachelor of Computer Science with Honours (Computational Science)  
Universiti Malaysia Sarawak (UNIMAS)

## Project Overview

This project develops a comparative forecasting framework for Malaysia's carbon dioxide (CO₂) emissions using statistical and machine learning models. The project compares ARIMA, Random Forest, and XGBoost models, then generates Business-as-Usual (BAU) and Low-Carbon Transition (LCT) projections for Malaysia.

The final outputs include model performance comparison, CO₂ emission forecasts, scenario-based projections, and a Power BI dashboard for visualising the results.

## Objectives

1. To construct a structured dataset on Malaysia's historical CO₂ emissions with relevant socioeconomic and energy-related variables.
2. To develop forecasting models to generate CO₂ emission forecasts for Malaysia.
3. To evaluate model performance using standard predictive accuracy metrics.

## Models Used

- **ARIMA**: Statistical baseline model using historical CO₂ emissions.
- **Random Forest Regressor**: Ensemble machine learning model using lagged CO₂, GDP, population, and energy-use variables.
- **XGBoost Regressor**: Boosting-based machine learning model used for final forecasting and scenario analysis.

## Dataset

The project uses secondary data from public data repositories:

- CO₂ emissions: Our World in Data (OWID)
- GDP: World Bank Open Data
- Population: World Bank Open Data
- Energy use: World Bank Open Data

The modelling dataset covers selected countries from 1990 to 2022, with model training performed on 1992 to 2019 and testing on 2020 to 2022.

## Repository Structure

```text
carbon-emission-forecasting-malaysia/
│
├── README.md
├── requirements.txt
├── .gitignore
│
├── notebooks/
│   ├── 01_data_preparation.ipynb
│   ├── 02_arima_model.ipynb
│   ├── 03_random_forest_xgboost.ipynb
│   └── 04_forecasting_scenario_analysis.ipynb
│
├── data/
│   ├── raw/
│   ├── processed/
│   └── README.md
│
├── models/
│   └── README.md
│
├── results/
│   └── README.md
│
├── dashboard/
│   └── README.md
│
├── docs/
│   ├── user_manual.md
│   └── methodology_summary.md
│
└── assets/
    └── README.md
```

## How to Run

1. Clone this repository:

```bash
git clone https://github.com/your-username/carbon-emission-forecasting-malaysia.git
cd carbon-emission-forecasting-malaysia
```

2. Install required Python libraries:

```bash
pip install -r requirements.txt
```

3. Run the notebooks in order:

```text
01_data_preparation.ipynb
02_arima_model.ipynb
03_random_forest_xgboost.ipynb
04_forecasting_scenario_analysis.ipynb
```

4. Open the Power BI dashboard file from the `dashboard/` folder if available.

## Evaluation Metrics

Model performance is evaluated using:

- Root Mean Squared Error (RMSE)
- Mean Absolute Error (MAE)
- Mean Absolute Percentage Error (MAPE)

## Scenario Analysis

Two forecast scenarios are included:

- **Business-as-Usual (BAU)**: Assumes historical trends continue.
- **Low-Carbon Transition (LCT)**: Assumes reduced energy use based on an annual efficiency-improvement factor aligned with low-carbon transition assumptions.

## Dashboard

The Power BI dashboard presents:

- Historical and forecasted CO₂ emissions
- Model performance comparison
- BAU vs LCT scenario comparison
- Interactive filters for model, scenario, and year

## Disclaimer

This repository is prepared for academic purposes as part of the FYP 2 symposium submission. The forecasts are based on historical datasets and modelling assumptions, and should not be interpreted as official government projections.

## Author

**Nur Balqis Shafiera Binti Yusry**  
Bachelor of Computer Science with Honours (Computational Science)  
Faculty of Computer Science and Information Technology  
Universiti Malaysia Sarawak
