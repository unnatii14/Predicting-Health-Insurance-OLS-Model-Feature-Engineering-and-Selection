# Predicting Health Insurance OLS Model, Feature Engineering and Selection Using VIF and Correlation

[![Python](https://img.shields.io/badge/Python-3.11-blue)](https://www.python.org/) 
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)

## Overview
Predict health insurance charges using **OLS regression** with feature engineering and multicollinearity handling. The project identifies key factors influencing insurance costs and builds accurate, interpretable models.

## Key Features
- Polynomial & interaction features: `bmi_sq`, `age_bmi`, `age_smoker`  
- Binary encoding: `smoker_bin`  
- Multicollinearity check using **VIF**  

## Models Evaluated
- Linear Regression  
- Ridge & Lasso Regression  
- Random Forest Regressor  
- Gradient Boosting Regressor  
- Support Vector Regressor (SVR)  

## Final Performance

| Model               | RMSE    | MAE     | R²     |
|--------------------|---------|---------|--------|
| GradientBoosting    | 4339.14 | 2472.15 | 0.879  |
| RandomForest        | 4503.91 | 2442.21 | 0.869  |
| Ridge               | 5861.62 | 4321.12 | 0.779  |
| Lasso               | 5873.68 | 4338.74 | 0.778  |
| LinearRegression    | 5873.72 | 4338.78 | 0.778  |
| SVR                 | 12864.59| 8581.01 | -0.066 |

**Conclusion:**  
Tree-based ensemble models (Gradient Boosting and Random Forest) clearly outperform linear models and SVR for this dataset.

## Usage
1. Clone the repo:  
   ```bash
   git clone https://github.com/your-username/health-insurance-ols.git
