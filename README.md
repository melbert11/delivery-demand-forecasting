# Delivery Demand Prediction

A small forecasting project that predicts daily delivery demand from delivery-logistics data.

## Project structure

```text
dataset/
├── delivery_logistics.csv       # Raw delivery records
└── cleaned_dataset.pkl          # Dataset currently used by the modeling notebook
notebooks/
├── 01_eda.ipynb                 # Data cleaning, exploration, and feature engineering
└── 02_model.ipynb               # Model training and evaluation
```

## Workflow

1. Open `notebooks/01_eda.ipynb` to inspect and clean the raw data.
2. Open `notebooks/02_model.ipynb` to split the daily data into training and test sets.
3. Compare the following forecasting models:
   - Naive forecast
   - 7-day moving-average forecast
   - ARIMA
   - Linear regression
   - Random forest regressor
   - Prophet

Models are evaluated on the final 30 days using MAE, RMSE, MAPE, and mean forecast error (MFE).

## Getting started

This project uses Python 3.13 or later and [uv](https://docs.astral.sh/uv/).

```bash
uv sync
uv run jupyter lab
```

Then open the notebooks in numerical order.
