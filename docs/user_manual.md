# User Manual

## Project Title

Carbon Emission Forecasting in Malaysia Using Machine Learning

## Purpose

This project forecasts Malaysia's CO₂ emissions using ARIMA, Random Forest, and XGBoost models. It also compares Business-as-Usual and Low-Carbon Transition scenarios through model outputs and a Power BI dashboard.

## Software Requirements

- Python 3.9 or above
- Google Colab or Jupyter Notebook
- Microsoft Power BI Desktop
- Required Python libraries listed in `requirements.txt`

## Running the Project

### Step 1: Prepare Dataset

Open and run:

```text
notebooks/01_data_preparation.ipynb
```

This notebook prepares the master dataset, applies preprocessing, creates lag variables, and exports training/testing files.

### Step 2: Run ARIMA Model

Open and run:

```text
notebooks/02_arima_model.ipynb
```

This notebook trains and evaluates the ARIMA baseline model.

### Step 3: Run Random Forest and XGBoost

Open and run:

```text
notebooks/03_random_forest_xgboost.ipynb
```

This notebook trains and evaluates the machine learning models.

### Step 4: Generate Forecasts and Scenarios

Open and run:

```text
notebooks/04_forecasting_scenario_analysis.ipynb
```

This notebook generates 2023–2030 forecast outputs and BAU/LCT scenario results.

### Step 5: View Dashboard

Open the `.pbix` file in the `dashboard/` folder using Power BI Desktop.

## Expected Outputs

- Model performance table
- Forecasted CO₂ emissions for 2023–2030
- BAU and LCT scenario comparison
- Power BI dashboard visualisation

## Troubleshooting

### Problem: File not found
Check that the dataset files are placed in the correct folder path.

### Problem: Library import error
Run:

```bash
pip install -r requirements.txt
```

### Problem: Power BI file does not refresh
Check that the CSV file paths in Power BI match the current folder location.
