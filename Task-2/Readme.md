# Unemployment Analysis and Prediction

## Project Overview

This project analyzes unemployment trends across different states and regions in India using unemployment datasets from 2019–2020. The analysis includes data cleaning, exploratory data analysis (EDA), statistical analysis, interactive visualizations, COVID-19 impact assessment, and machine learning-based unemployment prediction.

The goal is to identify unemployment patterns, understand regional disparities, compare rural and urban unemployment, and build predictive models that estimate unemployment rates using socioeconomic indicators.


## Objectives

- Analyze unemployment trends across Indian states.
- Study the impact of COVID-19 on unemployment.
- Compare unemployment in rural and urban areas.
- Visualize employment and labor participation patterns.
- Identify states with high unemployment rates.
- Build machine learning models for unemployment prediction.
- Deploy an interactive prediction system using Gradio.


## Project Structure

Unemployment-Analysis/
│

├── data/

│   ├── Unemployment in India.csv

│   └── Unemployment_Rate_upto_11_2020.csv

│

├── notebooks/

│   └── unemployment_analysis.ipynb

│

├── models/

│   ├── random_forest_model.pkl

│   ├── xgboost_model.pkl

│   ├── region_encoder.pkl

│   └── area_encoder.pkl

├── requirements.txt

└── README.md

## Dataset

The project uses two datasets:

### Unemployment in India.csv

Contains:

- Region (State)
- Date
- Area (Rural/Urban)
- Estimated Unemployment Rate (%)
- Estimated Employed
- Estimated Labour Participation Rate (%)

### Unemployment_Rate_upto_11_2020.csv

Contains:

- Region
- Date
- Estimated Unemployment Rate (%)
- Estimated Employed
- Estimated Labour Participation Rate (%)
- Geographical Information

Dataset Source: Kaggle Unemployment in India Dataset


## Technologies Used

### Programming Language

- Python

### Libraries

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Plotly
- Scikit-Learn
- XGBoost
- Joblib
- Gradio


## Exploratory Data Analysis

The following analyses were performed:

### Data Cleaning

- Handling missing values
- Date conversion
- Column standardization
- Feature extraction

### Statistical Analysis

- Unemployment statistics
- Employment statistics
- Labour participation analysis
- Correlation analysis

### Visualizations

- Bar Charts
- Line Charts
- Histograms
- Box Plots
- Violin Plots
- Scatter Plots
- Correlation Heatmaps
- Sunburst Charts
- Choropleth Maps



## COVID-19 Impact Analysis

The project investigates the effect of COVID-19 lockdowns on unemployment rates.

### Key Observation

A significant increase in unemployment was observed during:

- April 2020
- May 2020

This indicates the economic impact of lockdown restrictions across India.


## Key Visualizations

### State-wise Unemployment Analysis

Identifies regions with the highest unemployment rates.

### Monthly Unemployment Trends

Tracks unemployment fluctuations over time.

### Rural vs Urban Comparison

Compares unemployment levels between rural and urban populations.

### Sunburst Visualization

Hierarchical visualization of:

Region → Area → Unemployment Rate

### Correlation Heatmap

Shows relationships among:

- Unemployment Rate
- Employment
- Labour Participation Rate

### India Choropleth Map

Visualizes unemployment distribution across Indian states.



## Machine Learning Models

Two regression models were developed:

### Random Forest Regressor

Used for:

- Non-linear relationships
- Feature importance analysis
- High prediction accuracy

### XGBoost Regressor

Used for:

- Gradient boosting
- Performance comparison
- Advanced predictive modeling



## Evaluation Metrics

Models were evaluated using:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score



## Gradio Web Application

An interactive Gradio interface was developed to predict unemployment rates based on:

- Region
- Area Type
- Month
- Year
- Estimated Employment
- Labour Participation Rate

### Features

- User-friendly interface
- Real-time predictions
- State selection dropdown
- Interactive inputs
- Instant unemployment rate estimation

## output
<img width="1366" height="697" alt="Image" src="https://github.com/user-attachments/assets/5ec9b395-d419-4aa4-a8fb-46cffdb62d5c" />
