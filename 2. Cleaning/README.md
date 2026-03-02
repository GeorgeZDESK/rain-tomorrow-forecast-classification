This folder contains the data preparation step of the project.

- `01_cleaning_export.ipynb`: loads the raw dataset from `../1. Data/weatherAUS.csv`, applies the agreed loose interpolation and feature engineering, then exports two files.
- Outputs are saved in `../1. Data/processed/`:
  - `weatherAUS_eda_ready.csv` for EDA and plots (keeps `Location`, `RainToday`, `Rainfall` for analysis-only use)
  - `weatherAUS_model_ready.csv` for modeling (drops leakage/unused columns and keeps only final features + target)

No modeling or hyperparameter tuning happens in this folder.