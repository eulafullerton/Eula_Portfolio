# Predicting Employment Status Among Foreign-Born Individuals

**Skills:** Logistic Regression | Census Data Analysis | Feature Interpretation | Classification Modeling

## Overview
Employment outcomes among foreign-born individuals vary due to differences in education, language ability, and time spent in the United States. This project analyzes demographic predictors of employment using American Community Survey data.

## Dataset
The analysis uses **2024 ACS Public Use Microdata (IPUMS)**.

The dataset was filtered to include **foreign-born individuals aged 18-64**.

Key variables included:

- Education level
- Years in the United States
- English proficiency
- Age
- Sex

The target variable was **employment status**.

## Methods
Logistic regression models were used to predict employment status.

Two models were compared:

- Baseline logistic regression
- Class-weighted logistic regression to address class imbalance

Evaluation metrics included:

- Accuracy
- Precision
- Recall
- F1-score

## Key Findings
Education level and years in the United States were the strongest predictors of employment outcomes among foreign-born individuals.
