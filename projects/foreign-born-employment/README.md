# Predicting Employment Status Among Foreign-Born Individuals

**Skills:** Logistic Regression | Census Data Analysis | Feature Interpretation | Classification Modeling

## Overview
This project analyzes demographic and socioeconomic predictors of employment among foreign-born individuals in the United States using American Community Survey (ACS) data.

## Dataset
The dataset used was the **2024 ACS Public Use Microdata Sample (IPUMS)**.

The analysis focused on foreign-born individuals aged 18–64.

Key variables included:

- Education level
- English proficiency
- Years in the United States
- Sex
- Age

The outcome variable was **employment status during the survey reference week**.

## Methods
A logistic regression model was used to predict employment status.

Two models were evaluated:

- Baseline logistic regression
- Class-weighted logistic regression to address class imbalance

Model performance was evaluated using:

- Accuracy
- Precision
- Recall
- F1-score

## Results
The baseline model achieved strong overall accuracy but performed poorly identifying not-employed individuals. Applying class weights improved recall for the minority class.

The strongest predictors of employment were:

- Education level
- Years in the United States

## Tools
Python, pandas, scikit-learn
