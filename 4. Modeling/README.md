This folder contains the machine learning work for predicting **RainTomorrow** (binary classification).

Inputs:
- `weatherAUS_model_ready.csv` (exported from the Cleaning step)

Contents:
- Notebooks that train and evaluate baseline models (e.g., Logistic Regression, Random Forest + SMOTE, Gradient Boosting + SMOTE)
- RandomForest + SMOTE tuning with `GridSearchCV`
- Operating-point selection via thresholding to prioritize **recall_1** and then maximize **precision_1**
- Final evaluation artifacts (metrics tables, ROC/PR curves, and confusion matrices)