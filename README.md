# Car Price Analysis Report

## Overview

This project investigates factors influencing the price of used cars. Using a dataset from Kaggle containing 426,000 car records (a subset of the original 3 million), the goal is to provide insights and recommendations for a used car dealership. The analysis follows the CRISP-DM framework for structured problem-solving.

---

## CRISP-DM Framework

### 1. Business Understanding
- **Objective**: Identify key features that influence a used car price
- **Client Goal**: Use these insights to adjust inventory pricing and improve marketing strategies.

### 2. Data Understanding
- **Dataset**: 426,000 entries of used car data.
- **Key Features Explored**: Brand, model, mileage, year, condition, location, and additional categories.

### 3. Data Preparation
- **Cleaning**: Handled missing values, outliers, and standardized data formats.
- **Feature Engineering**: Created new variables for age and imputed missing values.

### 4. Modeling
- **Approach**: Explored regression and classification models to predict car prices.
- **Techniques Used**: Linear Regression, Ridge Regression, and Lasso Regression with hyperparameter tuning using GridSearchCV.
- **Dimensionality Reduction**: Used Truncated SVD to reduce feature space and analyze key contributors.
- **Evaluation Metrics**: Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and R-squared.

### 5. Evaluation
- **Key Insights**:
  - Age and mileage are strong predictors of price.
  - Nonstandard fuel (electric) vehicles strongly impact price
  - Geographical factors such as state significantly influence pricing.

### 6. Deployment
- **Recommendations**:
  - Highlight features like low mileage, recent model years, and non-gas vehicles in marketing materials.
  - Focus inventory sourcing on popular manufactueres with high consumer demand.
---

## Results Summary
- **Top Predictors of Price**: Vehicle age, mileage, brand, condition, and transmission type.
- **Model Evaluation**:
  - **Best Model**: Ridge Regression, which outperformed others with the lowest Mean Squared Error (MSE) of approximately 98,291,640 and the lowest Mean Absolute Error (MAE) of 7,635.42.
  - **Other Models**: Linear Regression and Lasso Regression showed higher error rates and lower R² scores.
- **Recommendations for Dealership**:
  - Optimize stock to include vehicles with attributes that drive higher consumer interest.
  - Use Ridge Regression for predictive pricing due to its balance of accuracy and robustness.
---
