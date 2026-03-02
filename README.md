# rain-tomorrow-forecast-classification

Predict whether it will rain **tomorrow** in Australia using an explainable machine learning approach.  
The project follows a clear workflow: **data → cleaning → EDA → modeling → explainability (SHAP) → presentation**.

## Dataset
- Source: *Rain in Australia* (Kaggle)  
  https://www.kaggle.com/datasets/jsphyg/weather-dataset-rattle-package/data
- Raw file placed at: `1. Data/weatherAUS.csv`

## Project structure
- `1. Data/`  
  Raw dataset and processed exports (`processed/`).
- `2. Cleaning/`  
  Data preparation and export of clean datasets used in later stages.
- `3. Analysis/`  
  Exploratory Data Analysis (EDA) and exported figures.
- `4. Modeling/`  
  Baseline and tuned RandomForest (with threshold selection) + artifacts and figures.  
  Includes SHAP explainability in `04_explainability_shap/`.
- `5. Presentation/`  
  Final presentation assets (figures used in the slides).

## Key outputs
- Clean datasets:
  - `1. Data/processed/weatherAUS_eda_ready.csv`
  - `1. Data/processed/weatherAUS_model_ready.csv`
- Modeling results (CSV/JSON):
  - `4. Modeling/artifacts/results_baseline.csv`
  - `4. Modeling/artifacts/results_final.csv`
  - `4. Modeling/artifacts/results_final_with_threshold.csv`
  - `4. Modeling/artifacts/rf_smote_threshold.json`
  - `4. Modeling/artifacts/rf_smote_tuned_best_params.json`
- Explainability (SHAP):
  - Notebook: `4. Modeling/04_explainability_shap/01_shap_rf_smote_tuned.ipynb`

## Environment
- Python: **3.11.14**
- Install (one of the following):
  - `pip install -r requirements.txt`
  - `conda env create -f environment.yml`