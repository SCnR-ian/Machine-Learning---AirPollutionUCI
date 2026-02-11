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
  
   - Observed strong correlation between gas concentrations and sensor readings

   - Noted skewed distribution in pollution variables

### Data Preprocessing

   - Time alignment and timestamp construction

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

      - Random Forest Regressor

      - Gradient Boosting Regressor
  
   2. Classification (Air Quality Levels)

      - Target: CO concentration

      - Classes: Low / Medium / High pollution

      - Models: Logistic Regression, Random Forest, Gradient Boosting     


### Evaluation 
