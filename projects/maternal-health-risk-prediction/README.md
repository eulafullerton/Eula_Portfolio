# Maternal Drug Exposure and Pregnancy Outcomes

**Skills:** Data Integration | API Data Retrieval | SQL Database Creation | Data Cleaning | Exploratory Data Analysis | Public Health Analytics | Python (pandas, SQLite)

## Overview
Medication use during pregnancy is a critical public health concern because certain drugs may affect maternal and infant health outcomes. This project investigates patterns of medication exposure during pregnancy by integrating multiple public health datasets. The goal is to explore relationships between pregnancy-related conditions, commonly used medications, and potential infant outcomes.

## Datasets
This analysis integrates multiple public data sources:

**CDC Natality Data**
- U.S. birth data containing maternal health indicators and infant outcomes.

**OpenFDA Drug Adverse Event API**
- Drug safety reports containing medication reaction information.

**Pregnancy Drug Category Data (Wikipedia)**
- Drug safety classifications used to categorize medications by pregnancy risk.

These datasets were combined to examine relationships between maternal conditions, medications used to treat those conditions, and observed health outcomes.

## Data Preparation
The project involved several data engineering steps:

- Importing natality and drug datasets
- Retrieving drug information from the **OpenFDA API**
- Creating a **SQLite database** to store and query the combined datasets
- Joining multiple tables using SQL queries
- Cleaning and transforming variables to prepare them for analysis

Because the natality dataset does not directly list medications used during pregnancy, drug exposure was inferred from known treatments associated with pregnancy-related conditions.

## Methods
The analysis focused on exploratory data analysis and visualization techniques to examine patterns in drug usage and maternal health outcomes.

Key steps included:

- SQL joins between drug data and maternal health data
- Frequency analysis of pregnancy-related drug reactions
- Visualization of reported drug reactions
- Comparative analysis of regional drug usage and infant mortality patterns

## Key Findings
Several medications were commonly associated with pregnancy-related conditions, including:

- **Insulin** for gestational diabetes
- **Labetalol** for pre-pregnancy hypertension
- **Ceftriaxone** for gonorrhea treatment

Regional patterns suggested:

- Higher ceftriaxone usage in southern regions
- Nicotine exposure present across all regions, with higher mortality rates observed in the South

However, because drug usage was inferred rather than directly observed in the natality dataset, the analysis cannot establish causal relationships between medications and health outcomes.

## Ethical Considerations
This project highlights important ethical considerations when integrating health datasets. Inferring drug exposure from medical conditions introduces potential bias and should be interpreted cautiously. All datasets used were publicly available and contained no personally identifiable information.

## Tools
Python, pandas, SQLite, OpenFDA API, matplotlib
