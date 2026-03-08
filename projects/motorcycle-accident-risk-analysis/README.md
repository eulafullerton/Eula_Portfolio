# Motorcycle Accident Risk Analysis (California)

**Skills:** Data Cleaning | Exploratory Data Analysis | Data Visualization | Large Dataset Processing | SQL/SQLite | Statistical Analysis | R (dplyr, ggplot2)

## Overview
Motorcycle accidents account for a significant portion of traffic injuries and fatalities each year. This project analyzes large-scale traffic collision data to identify demographic, environmental, and temporal patterns associated with motorcycle accidents. The goal is to uncover patterns that may inform safety interventions and policy improvements.

## Motivation
As a night-shift medical laboratory scientist, I frequently encounter trauma cases resulting from motorcycle accidents. This exposure motivated an investigation into whether large-scale traffic datasets could reveal patterns associated with higher accident risk or severity.

## Datasets
This analysis integrates **three public transportation datasets**:

**1. California Traffic Collision Data (SWITRS)**
- 9.4 million collision records
- 18.7 million involved parties
- Variables include vehicle type, road conditions, lighting, injury severity, and rider demographics.

**2. Road Traffic Injury Dataset**
- 449,850 observations
- Contains injury and fatality statistics across transportation modes.

**3. U.S. Transportation Accident Data**
- National crash statistics from 1988–2022.

## Data Preparation
Data preparation involved several steps:

- Importing large datasets including **SQLite traffic collision data**
- Filtering relevant motorcycle-related records
- Joining collision and party tables
- Replacing missing values with standardized labels
- Removing duplicate observations
- Preparing variables for exploratory analysis

Handling large datasets required memory management and selective filtering to focus on motorcycle-related incidents.

## Analysis Methods
The analysis focused on **exploratory data analysis and statistical comparisons**, including:

- Age distribution analysis
- Gender comparisons
- Environmental condition analysis (lighting, weather, road conditions)
- Mode-of-transport comparisons
- Injury and fatality rate calculations

Visualization techniques included:

- Bar charts
- Histograms
- Boxplots
- Comparative mode-of-transport charts

## Key Findings

### Fatality Risk
Motorcycle accidents resulted in fatalities approximately **3.2% of the time**, with injuries occurring in **82% of cases**.

### Age Patterns
Younger riders, particularly those **in their twenties and early thirties**, were involved in the highest number of accidents.

### Gender Differences
Motorcycle accidents were heavily skewed toward **male riders**, though some records contained unknown gender classifications.

### Environmental Conditions
Contrary to common assumptions, most motorcycle accidents occurred under **normal weather, road, and lighting conditions**, suggesting that rider behavior and traffic interactions may be more influential than environmental conditions.

### Comparison to Other Modes
Motorcycle accidents produced a **higher injury rate than trucks, buses, and bicycles**, but slightly lower than cars and pedestrians in overall injury distribution.

## Implications
The findings highlight potential areas for safety intervention:

- Targeted rider safety programs for younger riders
- Improved rider training and licensing requirements
- Enhanced data collection for rider demographics
- Infrastructure and safety initiatives focused on motorcycle riders

## Tools
R, ggplot2, dplyr, tidyr, RSQLite, readxl
