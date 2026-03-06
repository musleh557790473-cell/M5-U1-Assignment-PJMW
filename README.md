# PJMW Hourly Energy Consumption — Time Series Analysis

A comprehensive time series analysis of PJM West Region hourly energy consumption data,
developed as part of Module 5 (Unit 1) of the Master's in AI for Construction &
Engineering (MAICEN1125) at Zigarat Institute.

## 📊 Dataset
- **Source:** [Kaggle — PJM Hourly Energy Consumption](https://www.kaggle.com/datasets/robikscube/hourly-energy-consumption)
- **File:** `PJMW_hourly.csv`
- **Coverage:** 2002–2018 | Hourly resolution | ~140,000+ records

## 🔬 Exercises Covered

| # | Topic | Method |
|---|-------|--------|
| 1 | Data Cleaning | Duplicate removal (`groupby`), missing value imputation (`ffill`) |
| 2 | Multi-Scale Visualization | Daily, weekly, and full-dataset plots |
| 3 | Seasonality Analysis | Hourly and weekday patterns using `pd.Categorical` |
| 4 | ACF / PACF Analysis | Statsmodels — hourly (lags=48) and daily (lags=30) |
| 5 | Prophet Forecasting | Facebook Prophet with `ParameterGrid` hyperparameter tuning |
| ★ | Bonus: SARIMA | `SARIMAX` + `itertools` grid search, best: SARIMA(2,0,3)(1,1,1,12) |

## 📈 Key Results
- **Prophet** — MAE: ~369 MW | MAPE: ~6.6%
- **SARIMA** — Best RMSE: 281.55 MW

## 🛠️ Libraries
`pandas` · `matplotlib` · `statsmodels` · `prophet` · `scikit-learn` · `tqdm`

## 🚀 Usage
Open in [Google Colab](https://colab.research.google.com/) and run all cells sequentially.
Upload `PJMW_hourly.csv` when prompted.

## Repository Structure

```
├── 00Data/          # Raw input data files (CSV, Excel, etc.)
├── 01Notebooks/     # Jupyter Notebooks for analysis
├── 02Results/       # Output files, charts, and visualizations
├── 03Docs/          # Documentation, reports, and references
└── README.md        # Project overview (this file)
```

## Files

| File | Location | Description |
|------|----------|-------------|
| `PJMW_Assignment_G6.ipynb` | `01Notebooks/` | Main analysis notebook |
| `PJMW_hourly.csv` | `00Data/` | Hourly data used for analysis |

## Group 6
