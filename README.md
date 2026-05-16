# BMI Predictors in PCOS: A Linear Regression Analysis

## Overview

This project uses multiple linear regression to identify clinical, hormonal, 
and lifestyle predictors of BMI in 539 women with and without PCOS from a 
retrospective clinical audit of 10 hospitals in Kerala, India.

## Data Source

- PCOS Dataset compiled by Kottarathil (Kaggle, 2020)
- 541 observations; 3 removed due to missing values (analytic N = 539)
- Variables span hormonal markers, clinical measures, and lifestyle indicators

Dataset is not included in this repository. Available at:  
https://www.kaggle.com/datasets/prasoonkottarathil/polycystic-ovary-syndrome-pcos

## Methods

- Descriptive statistics and bivariate correlation analysis
- Multiple linear regression with AIC and BIC stepwise model selection
- HC3 heteroscedasticity-consistent standard errors
- Regression diagnostics: residual plots, Shapiro-Wilk, Breusch-Pagan
- Influential observation analysis: Cook's Distance, DFBETAs
- Interaction analysis: PCOS × Cycle Regularity
- Predicted BMI profiles with 95% prediction intervals

## Key Findings

- Weight gain was the dominant predictor: women reporting recent weight gain 
  had BMI approximately 3.5 kg/m² higher on average
- PCOS diagnosis was not an independent predictor once hormonal and lifestyle 
  covariates were controlled, suggesting mediation through insulin resistance
- TSH showed a statistically significant but influential-observation-sensitive 
  association and should be treated as exploratory
- Model explained approximately 23% of BMI variance (Adj. R² = 0.229)

## Files

- `PCOS_BMI_Final_V.Rmd`: Fully reproducible R analysis
- `PCOS_BMI_Final_V.pdf`: Final rendered report

## Tools

- R: tidyverse, sandwich, lmtest, MASS, car

## Authors

Rohit Kambala, Navjot Kaur  
GPH-GU 2338: Linear Regression and Modeling  
MPH Biostatistics, New York University