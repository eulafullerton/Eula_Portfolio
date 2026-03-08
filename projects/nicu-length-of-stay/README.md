# Predicting NICU Length of Stay Using Admission Clinical Data

**Skills:** Machine Learning | Regression Modeling | Healthcare Analytics | Feature Engineering | Model Evaluation


## Overview
This project investigates whether clinical and demographic variables available at NICU admission can be used to predict neonatal length of stay (LOS). Accurate LOS predictions could help hospitals anticipate bed utilization, staffing needs, and operational planning in neonatal intensive care units.

## Dataset
The dataset used was the Neonatal Sepsis Care dataset containing neonatal clinical and demographic information collected at NICU admission.

Key variables included:

- Birth weight
- Gestational age
- Sex
- Delivery mode
- Maternal health indicators
- Apgar score
- Clinical symptoms such as respiratory distress and fever

The target variable was **length of stay in days**.

## Methods
Three regression models were evaluated:

- Linear Regression
- Gradient Boosting Regressor
- XGBoost Regressor

Data preparation included:

- One-hot encoding of categorical variables
- Log transformation of the LOS variable to reduce skewness
- Train/test split (80/20)

Models were evaluated using:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² score

## Results
All models produced similar performance with an average prediction error of approximately **4 days**. However, negative R² values indicated that admission-only variables did not capture enough information to explain variation in NICU length of stay.

Feature importance analysis showed that:

- Gestational age
- Birth weight
- Severity classification
- Admission temperature

were the most influential predictors.

## Tools
Python, pandas, scikit-learn, XGBoost, matplotlib
