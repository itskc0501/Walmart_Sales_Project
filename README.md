# Walmart Sales Project

Exploratory Data Analysis and Sales Prediction for Walmart — Krishna Chaitanya N

## Aim

- Establish and find relations between existing attributes of the dataset and see how each individual attribute affects sales.
- Get a store-wise analysis and find trends in the patterns.
- Build ML/ARIMA based prediction models to forecast future sales.
- Get a logical explanation for the current sales pattern and brainstorm ideas to improve upon it.

## Project structure

```
Walmart_Sales_Project/
├── data/
│   └── walmart.csv                     # raw dataset
├── notebooks/
│   ├── eda_sales_prediction.ipynb      # main EDA and forecasting notebook
│   └── schema.ipynb                    # dataset schema/feature descriptions
├── eda-sales-prediction-for-walmart.pdf  # exported report
├── requirements.txt
└── .gitignore
```

## Dataset

`data/walmart.csv` contains weekly sales for 45 Walmart stores over 2010-2012, with features:
`Store`, `Date`, `Weekly_Sales`, `Holiday_Flag`, `Temperature`, `Fuel_Price`, `CPI`, `Unemployment`.

Source: Kaggle. License: [CDLA Permissive 1.0](https://cdla.io/permissive-1-0/).

## Setup

```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1
pip install -r requirements.txt
```

## Usage

Open `notebooks/eda_sales_prediction.ipynb` in VS Code/Jupyter and run the cells in order. The notebook loads data via a path relative to the project root (`data/walmart.csv`); the included `.vscode/settings.json` keeps the notebook's working directory at the project root so this resolves correctly regardless of which folder the notebook lives in.
