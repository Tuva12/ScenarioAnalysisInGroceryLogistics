# Bachelor Project – Scenario Analysis in Grocery Logistics

This repository contains the code used in my bachelor thesis.
The project studies how delivery planning can be improved using prediction and optimisation.

## What the notebooks do

### 1 data_cleaning.ipynb
Cleans and prepares the data.

### 2 EDA.ipynb
Explores the data and shows patterns.

### 3 Feature Engineering.ipynb
Creates variables for the models.

### 4 linear regression model.ipynb
Builds a simple baseline model.

### 5 TFT_model.ipynb
Trains a machine learning model (TFT) to predict service time.

### scenario 1.ipynb
Tests normal route planning.

### scenario 2.ipynb
Tests higher volume (more goods).

### scenario 3.ipynb
Tests fewer vehicles.

## Method

The project uses a predict-then-optimise approach:
1. Predict service times
2. Use predictions in route planning
3. Test different scenarios

## Tools

- Python
- Pandas
- Scikit-learn
- PyTorch
- OR-Tools

## Note

The data is not included because it is based on real company data.
