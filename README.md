# Data Analysis and Regression Modeling

This repository contains a comprehensive analysis and regression modeling for the Combined Cycle Power Plant Data Set. The dataset includes hourly average readings of environmental conditions and their impact on the net hourly electrical energy output (EP) of the plant.

---

## Table of Contents

- [Introduction](#introduction)
- [Data](#data)
- [Project Tasks](#project-tasks)
  - [Exploring the Data](#exploring-the-data)
  - [Simple and Multiple Linear Regression](#simple-and-multiple-linear-regression)
  - [Nonlinear Associations](#nonlinear-associations)
  - [Interactions and Model Improvement](#interactions-and-model-improvement)
  - [KNN Regression](#knn-regression)
- [Results](#results)

---

## Introduction

This project involves analyzing and modeling the **Combined Cycle Power Plant** dataset to predict the net hourly electrical energy output (EP) using four environmental predictors. The models explored include linear regression, polynomial regression, interaction-based regression, and k-nearest neighbor (KNN) regression.

---

## Data

The dataset contains data points collected from a Combined Cycle Power Plant over six years (2006-2011).

### Features:
1. **Temperature (T)**: Hourly average ambient temperature (°C).
2. **Ambient Pressure (AP)**: Hourly average ambient pressure (millibar).
3. **Relative Humidity (RH)**: Hourly average relative humidity (%).
4. **Exhaust Vacuum (V)**: Hourly average exhaust vacuum (cm Hg).
5. **Electrical Energy Output (EP)**: Net hourly electrical energy output (MW) (Response Variable).

---

## Project Tasks

### Exploring the Data
1. **Data Dimensions**:
   - Count the number of rows (data points) and columns (variables).
   - Understand the meaning of rows and columns.
2. **Scatterplots**:
   - Generate pairwise scatterplots for all variables, including the response variable (EP).
   - Analyze trends and relationships.
3. **Summary Statistics**:
   - Compute mean, median, range, quartiles, and interquartile ranges for each variable.
   - Present the statistics in a table format.

### Simple and Multiple Linear Regression
1. **Simple Linear Regression**:
   - Fit a separate linear regression model for each predictor against the response (EP).
   - Analyze statistical significance and identify potential outliers.
   - Create plots for visualization.
2. **Multiple Linear Regression**:
   - Fit a regression model using all predictors.
   - Test for statistical significance of each predictor and interpret results.
3. **Comparison**:
   - Compare univariate regression coefficients with multiple regression coefficients.
   - Create a scatterplot with univariate coefficients on the x-axis and multiple regression coefficients on the y-axis.

### Nonlinear Associations
1. Fit polynomial regression models of the form:
   - Y = β₀ + β₁X + β₂X² + β₃X³ + ε
   - Assess the presence of nonlinear relationships for each predictor.

### Interactions and Model Improvement
1. **Interaction Terms**:
   - Fit a regression model including all pairwise interaction terms.
   - Determine statistical significance of interaction terms.
2. **Improved Model**:
   - Train a regression model with all predictors, interaction terms, and quadratic nonlinearities.
   - Use a subset (70% of the data) for training and the remaining data for testing.
   - Eliminate insignificant variables using p-values while preserving significant interactions.
   - Report train and test MSEs.

### KNN Regression
1. **KNN Modeling**:
   - Perform k-nearest neighbor regression using both raw and normalized features.
   - Identify the optimal \( k \in \{1, 2, ..., 100\} \) by minimizing the test error.
   - Plot train and test errors as functions of \( 1/k \).
2. **Comparison**:
   - Compare the results of KNN regression with the best-performing linear regression model.
   - Provide a detailed analysis of differences.

---

## Results

- **Exploratory Data Analysis**:
  - Visualizations and summary statistics provide insights into relationships and trends.
- **Simple vs. Multiple Regression**:
  - Comparison reveals the impact of multicollinearity and interaction terms.
- **Nonlinear and Interaction Models**:
  - Evidence of nonlinear relationships and interactions improves model performance.
- **KNN Regression**:
  - Optimal \( k \) identified, with comparisons to linear regression.

---
