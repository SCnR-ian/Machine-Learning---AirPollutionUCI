# Forecasting Air Pollution with Machine Learning

## Overview
   This project is an **end-to-end machine learning system** for **forecasting air pollution levels** using multivariate time-series sensor data.

   The goal is to build robust predictive models that capture **temporal dynamics, environmental influences, and real-world data issues** such as missing values, noise, and concept drift.

   The project demonstrates practical skills in **data preprocessing, feature engineering, time-series modeling, and model evaluation.**

## Objectives

   - Analyze air quality data

   - Perform **data cleaning** and **exploratory data analysis (EDA)**

   - Visualize pollution trends over time and across locations

   - Build machine learning models to predict air pollution levels

   - Evaluate model performance using appropriate metrics

  
## Process

### Exploratory Data Analysis

   - Identified -200 as missing value marker across features
  
   - Nonlinear Relationship Between Sensor Responses and True Concentrations (CO(GT) vs PT08.S1(CO): 0.04)

   - Inverse Sensor Responses (PT08.S3(NOx) vs NOx(GT): –0.44)
  
   - Sensors are highly correlated with each other (PT08.S1(CO) vs PT08.S2(NMHC): 0.93, PT08.S1(CO) vs PT08.S5(O3): 0.89)
  
   - Conclusion : Preference for tree-based and nonlinear models over purely linear approaches

### Data Preprocessing

   - Replace Nan with linear-based interpolation
  
   - Missing value handling and normalisation

   - Temporal feature extraction (hour, weekday, month)

### Feature Engineering

   - Lagged variables to capture temporal dependence

   - Rolling statistics (moving averages)

   - Comparison of short-term vs long-term temporal context

### Anormaly Detection

   - Residual-based anomaly detection to identify pollution spikes

   - Analysis of abnormal events and potential sensor faults

   - Evaluation using precision–recall trade-offs

### Machine Learning Models

   1. Regression (Pollutant Forecasting)
   
      - Linear Regression

      - Gradient Boosting Regressor
  
   2. Classification (Air Quality Levels)

      - Target: CO concentration

      - Classes: Low / Medium / High pollution

      - Models: Logistic Regression, Random Forest, Gradient Boosting     


### Evaluation 
   1. Regreesion

      - RMSE, R squared
  
   2. Classification

      - Confusion Matrix

      - Precision, Recall, F1-Score


