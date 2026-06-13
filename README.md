# Temperature Forecasting in Bern 

## Machine Learning course project - GSEM, University of Geneva (Prof. Sebastian Engelke, Fall 2025)

This repository contains the code for a graduate-level Machine Learning project focused on predicting the temperature in Bern, Switzerland, using meteorological observations from multiple weather stations.

## Project Objective

The objective of this project is to predict the temperature in Bern for three forecasting horizons:

* 12 hours ahead
* 24 hours ahead
* 48 hours ahead

The prediction task is based on meteorological observations collected from 10 weather stations across Switzerland. The project compares several machine learning models with different levels of complexity, interpretability, and predictive performance.

## Project Overview

Weather forecasting in Switzerland is challenging due to the country's geographical diversity, alpine regions, lake-adjacent areas, and local microclimates. These conditions create complex spatial and temporal relationships between meteorological variables.

The project includes exploratory data analysis, preprocessing, feature engineering, model training, model evaluation, and comparison of forecasting performance.

## Dataset Overview

The dataset includes meteorological measurements from 10 Swiss weather stations. The available variables include:

* Temperature
* Humidity
* Wind speed and wind gusts
* Atmospheric pressure
* Precipitation
* Radiation and sunshine duration
* Seasonal and temporal variables

The target variables are the future temperatures in Bern at 12-hour, 24-hour, and 48-hour forecasting horizons.

Raw data files are not included in this repository due to course and data-access restrictions.

## Methodology

The project workflow includes:

1. Data loading and overview
2. Exploratory data analysis
3. Missing value treatment
4. Outlier analysis
5. Target variable analysis
6. Correlation analysis
7. Feature engineering
8. Train/test splitting
9. Model fitting
10. Model comparison
11. Final model selection

## Models Used

The following models were implemented and compared:

* K-Nearest Neighbors
* Linear Regression
* Lasso Regression
* Ridge Regression
* Gradient Boosting
* XGBoost
* Bagging
* Random Forest
* Deep Neural Network

## Evaluation Metric

The main evaluation metric is Mean Absolute Error (MAE), which measures the average absolute difference between predicted and observed temperatures.

The models were evaluated separately for the 12-hour, 24-hour, and 48-hour forecasting horizons.

## Main Results

XGBoost was the best model across all horizons (Kaggle MAE ≈ 1.77 °C), confirming that
models able to capture non-linear interactions are best suited to this problem.

## Files
- `temperature_forecasting.ipynb` - main notebook (EDA, preprocessing, models)
- `neural_network.ipynb` - neural network (appendix)
- `report.pdf` - full project report


## Tools

* Python

## Authors
Group project (3 members): Zahra Ghafghazi, Aya Markous, Drenusha Fazlija.
Work was divided by model family and reviewed jointly by the team.
