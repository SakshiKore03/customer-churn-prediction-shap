# Customer Churn Prediction with Explainable AI

Predicts which telecom customers are likely to leave, and explains why using SHAP.

## Dataset
Telco Customer Churn (about 7,000 customers)

## Approach
- Cleaned the data and encoded categorical features
- Trained an XGBoost classifier with class weighting for the imbalanced churn data
- Used SHAP to explain which factors drive churn

## Results
- ROC-AUC: 0.834
- Recall for churners: 0.78
- Precision for churners: 0.49

I optimised for recall because missing a customer who is about to leave costs more than sending a retention offer to someone who would have stayed.

## Tech stack
Python, XGBoost, SHAP, Pandas, scikit-learn
