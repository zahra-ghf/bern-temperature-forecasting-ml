# Bern Temperature Forecasting with Machine Learning

## Machine Learning Course Project

This repository contains the code for a graduate-level Machine Learning project focused on predicting the temperature in Bern, Switzerland, using meteorological observations from multiple weather stations.

The project was developed as part of the Machine Learning course at the University of Geneva.

## Course Information

* Course: Machine Learning
* Institution: University of Geneva
* Semester: Fall Semester 2025
* Professor: Prof. Sebastian Engelke

## Team Members

This project was completed as a team project by:

* Zahra Ghafghazi
* Drenusha Fazlija
* Aya Markous

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

## Feature Engineering

Several feature engineering techniques were applied to improve model performance:

* Median imputation for missing values
* Standardization of predictors
* Cyclical encoding of the hour variable using sine and cosine transformations
* One-hot encoding of season
* Polynomial features for selected temperature variables
* Interaction terms between Bern temperature and neighboring station temperatures
* Additional spatial, temporal, and meteorological features

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

XGBoost achieved the best overall performance across all three forecasting horizons.
The results show that boosting-based models are well suited to capturing the nonlinear relationships and interactions present in meteorological data.

## Repository Structure

```text
.
├── README.md
├── notebooks/
│   ├── ML_ZAD_Project_2025.ipynb
│   └── DNN_Appendix_ZAD_Project_2025.ipynb
└── data/
    └── README.md
```

## Tools and Libraries

* Python
* Jupyter Notebook
* pandas
* NumPy
* scikit-learn
* XGBoost
* TensorFlow / Keras
* Matplotlib
* Seaborn
* GeoPandas

## Notes

The raw dataset and competition-specific documents are not included in this repository due to course and data-access restrictions.

This repository is intended to document the modeling workflow, feature engineering process, model comparison, and final forecasting approach used in the project.
