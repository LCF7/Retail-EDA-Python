# Exploratory Data Analysis for a Retail Company

## Table of Contents

- [Executive Summary](#executive-summary)
- [Objective](#objective)
- [Data Overview](#data-overview)
- [Data Sanity Test](#data-sanity-test)
- [Descriptive Statistics](#descriptive-statistics)
- [Key Findings](#key-findings)
- [Conclusions](#conclusions)
- [Repository Contents](#repository-contents)


## Executive Summary

This repository contains an Exploratory Data Analysis (EDA) performed on a dataset provided by a retail company, aimed at uncovering insights into the performance and adoption rates for membership in various stores within a retail chain. This analysis describes historical data to help define acceptable KPI metrics for conversion and adoption rates across different stores.

## Objective

The objective of this EDA is to identify the correlation between conversion and adoption rates and understand the general performance of the stores across the country.

## Data Overview

The dataset comprises 300 records with the following columns:
- `store_id`: Identifier for each store
- `week`: Week number (1 to 5)
- `conversion_rate`: Conversion rate (0.011 to 0.419)
- `adoption`: Adoption rate (0.003 to 0.966)
- `province`: Province where the store is located (ON, BC, AB)

## Data Sanity Test

- The dataset contains 300 rows and 5 columns.
- There are no null or missing values present.
- Provinces: 3 unique values (ON, BC, AB).
- Stores: 60 unique stores.
- Outliers were identified using the 1.5 IQR methodology.

## Descriptive Statistics

Key statistical measures and visualizations were used to understand the distribution and central tendencies of conversion and adoption rates.

## Key Findings

### Conversion Rate Distribution

![Conversion Rate](https://drive.google.com/uc?export=view&id=1euVV2qICNw1GAUmnMy4bvSiOjLXwIui6)  
- Normal distribution observed.
- Most conversion rates fall between 0.1 and 0.3.
- No outliers detected.
- Alberta (AB) has the highest average conversion rate (0.24497).

### Adoption Rate Distribution

![Adoption Rate ](https://drive.google.com/uc?export=view&id=1Oqa93Ka65zTba0zFzbjihe1_cV-s4-ye) 
- Right-skewed distribution, indicating most stores have lower adoption rates with a few exceptions.
- Outliers are present.
- Alberta (AB) leads with an average adoption rate of 0.31796.

### Store and Week Analysis
- Weeks 2 and 4 show the highest conversion rates.
- Weeks 3 and 4 have the highest adoption rates.
- No strong correlation between adoption and conversion rates.

### Correlation Analysis

![Correlation Analysis](https://drive.google.com/uc?export=view&id=1asxtsRu0b2P0iBLd1JqaBSQ8sBYISIYB) 
- Positive but weak correlation between adoption and conversion rates (R² = 0.105).
- Linear regression equation: y = 0.7963x + 0.1019 (not recommended for predictions).

## Conclusions

### Conversion Rates by Province
- Alberta's strategies appear more effective; Ontario and British Columbia's rates are significantly lower.
- Analysis of Alberta's strategies could provide insights for improvement in other provinces.

### Adoption Rate Analysis
- Alberta leads in adoption rates; similar performance gaps exist as with conversion rates.

### Weekly Analysis
- Identifying external factors or promotional activities could help explain variations.

### Performance Improvement
- Set metrics of top-performing stores as targets.
- Review lowest-performing stores for issues and areas for improvement.

### Correlation and Model Reliability

![Correlation and Model Reliability](https://drive.google.com/uc?export=view&id=1ZNMm4IRE0gE2jfbjEUCvPkerb6e4QIsN) 
- Weak relationship between conversion and adoption rates suggests caution in using the model for predictions.

## Repository Contents

- `EDA_Retail.ipynb`: Jupyter notebook containing the EDA.
- `EXPLORATORY DATA ANALYSIS.pdf`: Detailed report of the EDA findings.
- `Retail_Location_Analysis.csv`: Dataset used for the analysis.


