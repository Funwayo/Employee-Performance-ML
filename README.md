# Predicting Employee Performance Using Workforce Behaviour and Organisational Characteristics

## Overview

This repository contains the analytical artefact developed for an MSc Data Science dissertation investigating employee-performance prediction using machine learning.

The project develops and evaluates a leakage-aware and explainable machine-learning framework, with particular consideration of predictive performance, predictor validity and model interpretability.

The analysis uses a publicly available synthetic employee-performance dataset containing 100,000 observations and 20 variables.

## Analytical Approach

The project combines:

- exploratory data analysis and data preparation;
- predictor-validity and potential leakage investigation;
- staged feature-removal and ablation analysis;
- comparative evaluation of five supervised classification algorithms;
- five-fold stratified cross-validation; and
- SHAP-based model explainability.

The five classification algorithms evaluated are:

- Logistic Regression
- Decision Tree
- Random Forest
- XGBoost
- Linear Support Vector Machine

## Repository Structure

The analytical workflow is organised across four Jupyter notebooks:

### 1. `01_Data_Understanding.ipynb`
Examines dataset structure, data quality, class distribution and initial predictor-target relationships.

### 2. `02_Data_Preprocessing.ipynb`
Performs data preprocessing and feature refinement and investigates potentially problematic predictors through staged feature-removal and ablation analysis.

### 3. `03_Machine_Learning_Model_Development.ipynb`
Develops and evaluates Logistic Regression, Decision Tree, Random Forest, XGBoost and Linear SVM models using a majority-class baseline, classification metrics, confusion matrices and five-fold stratified cross-validation.

### 4. `04_Explainable_Artificial_Intelligence.ipynb`
Applies global, class-specific and local SHAP analysis to examine how retained predictors contribute to model outputs.

## Dataset

The project uses the publicly available **Employee Performance Dataset** by Ziya (2025), available through Kaggle.

The dataset is synthetic and contains 100,000 employee observations and 20 variables. The target variable, `Performance_Score`, contains five performance categories.

## Reproducibility

The notebooks are numbered according to the analytical workflow and should be reviewed in numerical order.

Consistent data partitions, experimental conditions and random states are used where applicable to support reproducibility.

## Important Interpretation

The project distinguishes predictive performance from predictor validity. A reduction in model performance following removal of a predictor is not treated independently as proof of target leakage.

Similarly, SHAP values are interpreted as explanations of fitted-model behaviour rather than evidence of causal relationships or validated determinants of employee performance.

## Dissertation

These notebooks provide the executable analytical evidence supporting the methodology and empirical results presented in Chapters 3 and 4 of the MSc Data Science dissertation:

**Predicting Employee Performance Using Workforce Behaviour and Organisational Characteristics: A Machine Learning Approach**
