# Diabetes Risk Prediction — NHANES 2017-2018

## Overview
Multiclass classification model predicting diabetes status 
(No Risk, Borderline, Diabetic) using real CDC NHANES survey data.

## Dataset
- Source: CDC NHANES 2017-2018
- 5,277 adult participants after cleaning
- 3 files merged: Demographics, Body Measures, Diabetes Questionnaire

## Features
- Age, Gender, Ethnicity, Height, BMI
- Engineered: Waist/Height ratio, BMI×Age

## Models Trained
- Logistic Regression — 60%
- Random Forest — 70%
- XGBoost — 80% ← best model

## Key Challenges
- Severe class imbalance (151 Borderline vs 4,356 No Risk)
- Real world messy data requiring extensive cleaning
- Avoiding data leakage from prior diagnosis columns

## What I Learned
...
