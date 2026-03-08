# Maternal Health Risk Prediction

**Skills:** Machine Learning | Classification | Feature Engineering | Model Comparison | Healthcare Analytics | Python (pandas, scikit-learn)

## Overview
Maternal health complications remain a significant global health concern. Early detection of high-risk pregnancies can improve prenatal care, enable early intervention, and reduce maternal and infant mortality.  

This project develops machine learning models to classify pregnancy risk levels using maternal health indicators. Risk levels were categorized as:

- Low Risk
- Mid Risk
- High Risk

The objective was to determine whether physiological measurements routinely monitored during pregnancy could accurately predict maternal risk levels.

## Dataset
The dataset was obtained from Kaggle and contains maternal health indicators commonly monitored during pregnancy.

Key variables included:

- Maternal age
- Systolic blood pressure
- Diastolic blood pressure
- Blood glucose level
- Body temperature
- Heart rate

The target variable was **RiskLevel**, representing pregnancy risk categories.

## Data Preparation
Several preprocessing steps were performed:

- Removal of **562 duplicate records**
- Correction of unrealistic values (heart rate outlier)
- Standardization of numerical features
- Encoding of risk categories:
  - Low Risk = 0
  - Mid Risk = 1
  - High Risk = 2

Exploratory data analysis included visualizations examining relationships between maternal age, blood pressure, glucose levels, and pregnancy risk.

## Feature Selection
A Random Forest model was used to evaluate feature importance. The most influential predictors were:

1. Blood glucose level  
2. Systolic blood pressure  
3. Maternal age  
4. Diastolic blood pressure  
5. Body temperature  

Heart rate was removed due to weak correlation with the target variable.

## Models Evaluated
This multi-class classification problem evaluated four machine learning models:

- Random Forest Classifier
- Support Vector Machine (SVM)
- XGBoost
- Logistic Regression

Model performance was compared using classification accuracy.

## Results

| Model | Accuracy |
|------|------|
| Random Forest | **70%** |
| SVM | 68% |
| XGBoost | 65% |
| Logistic Regression | 64% |

The Random Forest model produced the highest predictive accuracy and was the most effective model for identifying high-risk pregnancies.

However, all models struggled to accurately classify **mid-risk pregnancies**, suggesting that additional clinical variables may be necessary for improved classification.

## Key Takeaway
Machine learning models show promise for predicting maternal health risk levels using physiological indicators collected during pregnancy. While the Random Forest model performed best in this analysis, additional clinical data and further validation would be required before real-world deployment.

## Tools
Python, pandas, scikit-learn, XGBoost, matplotlib
