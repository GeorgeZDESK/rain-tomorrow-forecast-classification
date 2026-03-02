This folder contains SHAP-based explainability for the final tuned model (**RandomForest + SMOTE**).

- `01_shap_rf_smote_tuned.ipynb`: Loads the saved tuned pipeline (`rf_smote_tuned.joblib`), rebuilds the same feature space (OHE), and computes SHAP values on a small test sample for speed.
- `../figures/shap/`: Exported SHAP plots (beeswarm + bar) styled to match the presentation theme.
- `../artifacts/shap/`: Exported SHAP tables (feature ranking by mean(|SHAP|), top features CSVs).

Notes:
- SHAP is computed for **class = 1 (Rain)** and uses a reduced sample size to avoid long runtimes.