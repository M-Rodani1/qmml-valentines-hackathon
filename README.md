#  Queen Mary Machine learning society Valentine's Day Hackathon 2026

**2nd place** | **0.59235 AUC** (1st: 0.59275)

Predict whether a person has a Valentine's date from demographic and social attributes. 700k train rows, evaluated on ROC-AUC.

## What I did

- Parsed `Survey_Date` into month/hour/day, created interaction terms, log-transformed income, added missingness flags
- Target encoded categoricals with KFold to avoid leakage
- Tuned LightGBM, XGBoost and CatBoost with Optuna (50 trials each)
- Rank-based ensemble of all three models

Link to hackathon kaggle: https://www.kaggle.com/competitions/valentines-hackathon/overview
