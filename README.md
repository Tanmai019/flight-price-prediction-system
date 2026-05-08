# Flight Price Prediction System

Machine learning pipeline for predicting U.S. airline ticket prices using statistical analysis, feature engineering, ensemble learning, and large-scale historical flight data.

This project analyzes airline fare trends from 1993–2024 and builds predictive models using regression and ensemble machine learning techniques to forecast flight prices and identify the key drivers influencing airline pricing.

---

# Tech Stack

`Python` `Scikit-learn` `XGBoost` `Random Forest` `Pandas` `NumPy` `Matplotlib` `Seaborn` `Machine Learning`

---

# Project Overview

The project explores historical airline fare data containing:

- 245,955 flight records
- 23 structured features
- multiple airline pricing indicators
- route-level and market-level information

The workflow combines:
- exploratory data analysis
- statistical preprocessing
- feature engineering
- regression modeling
- ensemble learning
- model evaluation

to build accurate fare prediction systems.

---

# Features

- Airline fare prediction
- Large-scale regression modeling
- Feature engineering workflows
- Ensemble learning pipelines
- Outlier detection and removal
- Statistical correlation analysis
- Feature importance analysis
- Model comparison framework

---

# Problem Statement

Airline ticket prices are influenced by several factors including:

- route distance
- seasonal demand
- passenger volume
- airline competition
- market share dynamics
- pricing strategies

The goal of this project is to model these relationships and accurately predict flight fares using machine learning.

---

# Dataset

The dataset contains:

- 245,955 flight records
- 23 features
- U.S. airline pricing data
- historical data from 1993–2024

Key variables include:
- fare
- distance (`nsmiles`)
- passenger count
- market share metrics
- carrier information
- seasonal and temporal indicators

---

# Machine Learning Models

The project evaluates multiple regression models:

- Linear Regression
- Support Vector Regression (SVR)
- K-Nearest Neighbors (KNN)
- Random Forest Regressor
- Gradient Boosting Regressor
- XGBoost Regressor
- Ensemble Voting Regressor

---

# Repository Structure

```text
flight-price-prediction-system/
├── Data_Cleaning_and_EDA.ipynb
├── VariableSelection.ipynb
├── ML_Models.ipynb
├── XGBoost_and_Ensemble_Model.ipynb
├── Bi_directional_elimination.ipynb
├── TestResults.ipynb
└── README.md
```

---

# Data Preprocessing

The preprocessing workflow includes:

- missing value handling
- grouped-value imputation
- categorical encoding
- outlier detection using IQR
- feature scaling
- feature selection

---

# Feature Selection Techniques

Several feature selection methods were explored:

- Correlation Matrix Analysis
- Lasso Regularization
- Forward Feature Selection
- Bidirectional Feature Selection

Key predictive features identified:

- `nsmiles`
- `fare_low`
- `fare_lg`
- `large_ms`
- `passengers`
- `lf_ms`

---

# Model Evaluation Metrics

Models were evaluated using:

- RMSE (Root Mean Squared Error)
- MAE (Mean Absolute Error)
- R² Score

---

# Key Results

## Linear Regression
- RMSE: `17.263`

## Support Vector Regression
- RMSE: `17.737`

## K-Nearest Neighbors
- RMSE: `14.674`

## Random Forest
- Test RMSE: `13.39`
- Test R²: `0.96`

## XGBoost
- Test RMSE: `12.93`
- Test R²: `0.961`

## Ensemble Model
- Best overall predictive performance
- Lowest RMSE
- Highest robustness across datasets

---

# XGBoost Insights

XGBoost delivered the strongest standalone model performance.

Important predictive features included:

- route distance (`nsmiles`)
- passenger volume
- market share metrics
- lowest available fares

The model demonstrated:
- low prediction error
- high R² performance
- stable residual distributions

---

# Ensemble Learning

The final ensemble model combined:

- Random Forest
- XGBoost

through a Voting Regressor framework to improve:
- prediction accuracy
- robustness
- generalization performance

The ensemble approach outperformed individual models by leveraging complementary learning behavior.

---

# Visualizations

The project includes:

- feature importance plots
- correlation heatmaps
- residual analysis
- actual vs predicted fare plots
- error distribution analysis
- exploratory data visualizations

---

# Example Workflow

Input:
- historical airline pricing data

Processing:
- preprocessing
- feature engineering
- model training
- hyperparameter tuning

Output:
- predicted airline fares
- feature importance insights
- model comparison metrics

---

# Skills Demonstrated

- Regression modeling
- Ensemble learning
- Feature engineering
- Statistical analysis
- Hyperparameter tuning
- Predictive analytics
- Machine learning experimentation
- Exploratory data analysis (EDA)

---

# Key Learnings

- Ensemble methods significantly improved predictive accuracy
- Route distance and market competition strongly influence pricing
- Feature engineering played a major role in model performance
- XGBoost provided strong scalability and robustness for structured airline data

---

# Limitations

- Some models required extensive hyperparameter tuning
- Historical pricing behavior may not fully reflect future airline market conditions
- The workflow is notebook-based rather than production packaged

---

# Future Improvements

- Convert notebooks into modular production pipelines
- Add real-time airline API integration
- Build interactive visualization dashboards
- Deploy prediction models through web applications
- Experiment with deep learning regression models

---

# Notes

- Large datasets were excluded from GitHub for repository optimization.
- The project was originally developed as part of an academic machine learning workflow and later cleaned into a portfolio-ready implementation.
- Notebook outputs were simplified before GitHub upload for readability.
