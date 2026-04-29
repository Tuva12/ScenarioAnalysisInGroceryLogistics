# Bachelor Project - Scenario Analysis in Grocery Logistics

This repository contains the code used in my bachelor thesis.
The project studies how delivery planning can be improved using prediction and optimisation.

## What the notebooks do

### 1 data_cleaning.ipynb
Cleans and prepares the raw delivery data. This includes standardising column names, converting date and time columns, removing invalid records, filtering weekday deliveries, and preparing the dataset for later analysis.

### 2 EDA.ipynb
Performs exploratory data analysis. This notebook investigates patterns in delivery service time, customer frequency, workload variables, weekday effects, and route identifier stability.

### 3 Feature Engineering.ipynb
Creates model features used for forecasting. This includes time-based variables, lag features, rolling statistics, customer-level ordering, and other variables used as input to the forecasting models.

### 4 linear regression model.ipynb
Implements a simple linear regression baseline model. The baseline is used to compare the performance of the Temporal Fusion Transformer models.

### 5 TFT_model.ipynb
Trains and evaluates the Temporal Fusion Transformer model for service-time forecasting. The notebook includes model configuration, training, validation, and forecasting performance evaluation.

### scenario 1.ipynb
Tests normal operations by reordering stops within existing delivery time windows using OR-Tools.

### scenario 2.ipynb
Tests a volume shock scenario where delivered volume increases at selected stops. The notebook evaluates whether re-optimisation can restore route feasibility under capacity constraints.

### scenario 3.ipynb
Tests a reduced fleet scenario where selected vehicles are removed and their workload is reassigned to remaining vehicles.


## Method

The project uses a predict-then-optimise approach:
1. Predict service times
2. Use predictions in route planning
3. Test different scenarios

## Tools

- pandas
- numpy
- matplotlib
- scikit-learn
- torch
- pytorch-lightning
- pytorch-forecasting
- ortools
- jupyter
- openpyxl
  
## Note

The data is not included because it is based on real company data.


## Prototype

The live prototype can be accessed here:
https://prototype-2rsyurwczp3rzb8f8kbpju.streamlit.app/

The source code repository is available here:
https://github.com/Tuva12/Prototype
