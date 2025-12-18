# Flight Price Prediction using Machine Learning

## Overview
This project focuses on predicting airline ticket prices using historical flight booking data. The objective is to build an accurate machine learning model that estimates flight prices based on airline, route, journey date, duration, and other relevant factors.

## Dataset
The dataset consists of historical flight information, including:
- Airline
- Source and destination
- Route
- Date and time of journey
- Duration
- Total stops
- Ticket price

## Problem Statement
Flight ticket prices vary significantly depending on multiple factors. This project aims to identify key price drivers and build a predictive model that can accurately estimate ticket prices for better planning and decision-making.

## Approach
- Separated training and testing datasets before preprocessing to prevent **data leakage**
- Data cleaning including:
  - Handling missing values
  - Removing duplicate records
  - Detecting and treating outliers
- Feature engineering:
  - Encoding categorical variables
  - Extracting features from date and time columns
- Exploratory Data Analysis (EDA) to understand relationships between variables
- Model training and comparison
- Hyperparameter tuning to optimize performance and avoid overfitting
- Feature importance analysis to identify key factors affecting flight prices

## Models Used
- Linear Regression
- Random Forest Regressor
- XGBoost Regressor

## Model Evaluation
Models were evaluated using regression metrics:
- RMSE (Root Mean Squared Error)
- MAE (Mean Absolute Error)
- R² Score

## Results & Conclusion
- Linear Regression showed poor performance due to high error and was not suitable for this problem.
- Random Forest provided strong baseline results, but hyperparameter tuning resulted in limited improvement.
- XGBoost outperformed all other models even without tuning.
- Tuned XGBoost achieved the **lowest RMSE and highest predictive accuracy**, making it the best-performing model and suitable for deployment.

This project received an **A++ grade** for end-to-end implementation, model selection, and evaluation.

## Feature Importance
Feature importance analysis was performed to identify the most influential factors affecting flight prices, helping improve model interpretability and decision-making.

## Tools & Technologies
- Python
- Pandas, NumPy
- scikit-learn
- XGBoost
- Matplotlib, Seaborn

## Key Learnings
- Importance of preventing data leakage in machine learning pipelines
- Impact of feature engineering on model performance
- Model comparison and selection based on appropriate evaluation metrics
- Effectiveness of ensemble methods like XGBoost for regression problems

## Future Improvements
- Model deployment using Flask or FastAPI
- Real-time price prediction interface
- Incorporation of additional features such as seasonality and demand trends
