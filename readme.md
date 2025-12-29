Linear Regression Analysis - Cancer Mortality Data
Overview
This project implements linear regression analysis to predict cancer mortality rates using county-level demographic and health data. The assignment demonstrates both simple and multivariable linear regression using Python's scientific computing stack.
Dataset
The analysis uses cancer_data_cleaned.csv, which contains:

Target Variable: TARGET_deathRate - Cancer mortality rate per 100,000 people
Key Predictor: incidenceRate - Mean cancer diagnoses per 100,000
Additional Predictors: 15 demographic and socioeconomic variables including:

Median income
Population estimates
Poverty percentage
Median age
Healthcare coverage statistics
Demographic composition



Dataset Size: 3,047 observations × 17 features
Implementation
Technologies Used

Python 3.x
Libraries:

pandas - Data manipulation and analysis
numpy - Numerical computing
matplotlib - Data visualization
scikit-learn - Machine learning models



Key Components
1. Data Loading and Exploration

Read CSV data using pandas
Display dataset structure and contents

2. Visualization

Created scatter plot of incidence rate vs. death rate
Added regression line to visualize linear relationship
Identified potential outliers affecting model fit

3. Simple Linear Regression

Built model using scikit-learn's LinearRegression
Features: Single predictor (incidenceRate)
Performance: R² ≈ 0.202

4. Manual Regression Calculations
Implemented custom functions to compute regression coefficients:

dotProduct(x, y) - Compute dot product of vectors
sumSquares(x) - Sum of squared elements
squareSum(x) - Square of summed elements
slope(x, y, n) - Calculate regression slope (β₁)
yIntercept(x, y, z) - Calculate y-intercept (β₀)
