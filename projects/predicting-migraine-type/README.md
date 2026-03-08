# Predicting Migraine Type from Patient Characteristics and Symptoms

**Skills:** Machine Learning | Classification | SMOTE | Model Comparison | Healthcare Analytics

## Overview
Migraines affect more than one billion people worldwide and are frequently misdiagnosed or undertreated. This project explores whether machine learning models can classify migraine types using patient symptom patterns and demographic characteristics.

## Dataset
The dataset contains **400 patient records with 23 features** describing migraine symptoms and episode characteristics.

Key variables include:

- Age
- Attack duration
- Attack frequency
- Pain intensity
- Associated symptoms such as nausea, photophobia, and phonophobia
- Neurological symptoms such as vertigo and visual disturbances

The target variable was **Migraine Type**, consisting of seven migraine categories.

## Methods
Three classification models were evaluated:

- Logistic Regression
- Random Forest
- XGBoost

Preprocessing included:

- Removing duplicates
- Label encoding migraine type
- Standardizing numerical features
- Applying **SMOTE** to address class imbalance
- Stratified 80/20 train-test split

Performance metrics included:

- Accuracy
- Macro and weighted F1-score
- ROC-AUC

## Key Findings
Tree-based models significantly outperformed logistic regression.

| Model | Accuracy |
|------|------|
| Logistic Regression | 80% |
| Random Forest | 90% |
| XGBoost | **91%** |

Important predictors included migraine intensity, attack duration, frequency, nausea, and visual disturbances.
