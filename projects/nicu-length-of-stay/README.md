# Predicting NICU Length of Stay Using Admission Clinical Data

**Skills:** Machine Learning | Regression Modeling | Healthcare Analytics | Feature Engineering | Model Evaluation

## Overview
Neonatal Intensive Care Unit (NICU) length of stay (LOS) directly affects hospital capacity planning, staffing allocation, and patient care coordination. This project evaluates whether clinical and demographic variables available at NICU admission can be used to predict length of stay using supervised machine learning models.

## Dataset
The analysis uses the **Neonatal Sepsis Care dataset**, containing clinical and demographic indicators recorded at NICU admission.

Key variables include:

- Gestational age
- Birth weight
- Sex
- Delivery mode
- Maternal health indicators
- Apgar score
- Clinical symptoms such as respiratory distress

The target variable was **length_of_stay_days**.

## Methods
Three regression models were evaluated:

- Linear Regression
- Gradient Boosting Regressor
- XGBoost Regressor

Data preparation included:

- One-hot encoding categorical variables
- Log transformation of LOS to reduce skewness
- Train/test split (80/20)

Model performance was evaluated using:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R²

## Key Findings
Models predicted LOS within roughly **4 days of actual stay**, but negative R² values indicated limited explanatory power. The most influential predictors included:

- Gestational age
- Birth weight
- Severity classification
- Admission temperature

These results suggest that **post-admission clinical progression likely plays a larger role in determining NICU length of stay than admission variables alone.**
