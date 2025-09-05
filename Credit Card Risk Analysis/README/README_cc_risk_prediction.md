# Credit Card Risk Prediction

## Overview
This notebook outlines the project team’s approach to predicting whether a customer requires attention based on their behavior and financial indicators.

## Key Steps
- Selected original numerical features and removed highly correlated/redundant ones using **correlation analysis** and **VIF**.
- Addressed class imbalance considerations (2.7:1 ratio).
- Split data into training (80%) and test (20%), and applied scaling.
- Trained logistic regression as a baseline model, with alternatives (MLP, RandomForest, XGBoost) considered.
- Evaluated results using Accuracy, F1-score, and cross-validation.

## Outcomes
- Logistic Regression achieved **83% F1 score** and **91% accuracy**.
- 5-fold cross-validation confirmed stable performance (~81% F1, low deviation).
- Logistic Regression deemed sufficient for risk flag forecasting.
