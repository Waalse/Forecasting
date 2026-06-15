# Drug Demand Forecasting

## Project Overview

This project forecasts future drug demand using synthetic monthly supply-chain data.

It compares traditional time-series models with machine-learning regression models and selects the best-performing model for each drug.

## Dataset

The dataset contains:

| Column | Description |
|---|---|
| `drug` | Synthetic drug identifier |
| `date` | Monthly observation date |
| `demand` | Monthly drug demand |
| `supply` | Monthly supplied quantity |
| `inventory` | Closing inventory quantity |
| `shortage` | Shortage indicator |

## Forecasting Models

The notebook compares:

- Seasonal Naive
- Exponential Smoothing
- SARIMA
- Random Forest
- Gradient Boosting

## Workflow

The notebook covers:

- Data loading and validation
- Monthly time-series preparation
- Historical demand visualization
- Lag and rolling-feature engineering
- Time-based train-test splitting
- Model training and evaluation
- Best-model selection for each drug
- Three-month demand forecasting
- Forecast visualization and export

## Model Evaluation

Models are compared using:

- Mean Absolute Error
- Root Mean Squared Error
- R-squared

The model with the lowest Mean Absolute Error is selected for each drug.

## Project Files

```text
drug-demand-forecasting/
├── drug_forecasting_data.csv
├── drug_demand_forecasting_with_time_series.ipynb
└── README.md
```

## How to Run

Install the required libraries:

```bash
pip install pandas numpy matplotlib scikit-learn statsmodels jupyter
```

Open the notebook in VS Code or Jupyter and run the cells in order.

## Skills Demonstrated

- Time-series forecasting
- Machine-learning regression
- Feature engineering
- Time-based model validation
- Model comparison
- Drug-level model selection
- Forecast visualization
- Results export

## Disclaimer

This project uses synthetic data and is intended for educational and portfolio purposes only.
