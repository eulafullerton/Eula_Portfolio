# Predicting Migraine Type from Patient Characteristics and Symptoms

**Skills:** Machine Learning | Classification | SMOTE | Model Comparison | Healthcare Analytics

## Overview
Migraines affect over one billion people worldwide and are a leading cause of disability. However, migraines are frequently underdiagnosed or misclassified, which can lead to ineffective treatment. This project explores whether machine learning models can accurately classify migraine types using patient characteristics and associated neurological symptoms.

## Dataset
The dataset was sourced from Kaggle and contains **400 patient records with 23 features** describing migraine characteristics and symptoms.

Key variables include:

- Age
- Migraine duration
- Attack frequency
- Pain intensity and location
- Associated symptoms such as nausea, photophobia, and phonophobia
- Neurological symptoms including vertigo, tinnitus, and visual disturbances

The target variable was **Migraine Type**, consisting of seven migraine categories.

## Data Preparation
Data preprocessing included:

- Removing duplicate records
- Encoding migraine type labels using LabelEncoder
- Standardizing numerical variables (age, intensity, duration, frequency)
- Handling class imbalance using **SMOTE**
- Splitting the dataset using **stratified 80/20 train-test sampling**

## Methods
Three supervised machine learning models were evaluated:

- Logistic Regression
- Random Forest
- XGBoost

Model performance was compared using:

- Accuracy
- Macro and weighted **F1-score**
- ROC-AUC scores
- Confusion matrices

Because the dataset contained class imbalance, macro F1-score was used to evaluate model performance across all migraine categories.

## Results

| Model | Accuracy | Macro F1 |
|------|------|------|
| Logistic Regression | 80% | 0.76 |
| Random Forest | 90% | 0.80 |
| XGBoost | **91%** | **0.84** |

Tree-based models significantly improved classification performance compared to logistic regression. **XGBoost achieved the best overall performance and demonstrated strong ability to identify minority migraine classes.**

Feature importance analysis from the Random Forest model identified key predictors including:

- Migraine intensity
- Attack duration
- Attack frequency
- Visual disturbances
- Nausea

These predictors align closely with clinical migraine symptom patterns.

## Key Takeaway
Machine learning models can effectively classify migraine types based on symptom patterns. XGBoost provided the strongest performance, suggesting that ensemble models are well suited for multi-class clinical classification tasks.

## Tools
Python, pandas, scikit-learn, XGBoost, SMOTE, matplotlib
