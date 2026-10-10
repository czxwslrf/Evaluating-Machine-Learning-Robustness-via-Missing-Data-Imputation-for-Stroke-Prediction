# Evaluating Machine Learning Robustness via Missing Data Imputation for Stroke Prediction

## Overview

This project investigates how different missing data imputation methods affect the performance of a Random Forest model for stroke prediction.

Three imputation methods are evaluated:

- K-Nearest Neighbours (KNN)
- Multiple Imputation by Chained Equations (MICE)
- MissForest

The experiments use missing data rates of 10%, 20%, and 30%, with five random seeds to generate different missing data patterns.

## Dataset

The project uses the **Stroke Prediction Dataset**, available on Kaggle:

https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset

## Methodology

A Random Forest classifier is trained on the cleaned dataset to establish baseline performance.

Missing values are then artificially introduced into the test dataset. Each imputation method is applied to reconstruct the missing values.

The methods are evaluated using:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- F1-score
- Robustness Score (Rq)

## Results

The experimental results are saved in the `results` folder, including individual results, summary statistics, and comparison figures.

## Purpose

This project was developed as part of an academic study investigating the robustness of machine learning models when handling missing data in stroke prediction.