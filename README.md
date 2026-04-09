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

1. The biggest difference between a Kaggle dataset and a real world 
dataset is how incomplete the data is and the importance of cleaning it properly.

2. I learned that data leakage is bad because the model will not be 
accurate in real world predictions. I avoided this by removing columns 
that revealed prior diabetes diagnoses.

3. I learned that class imbalance happens when the model doesn't have 
enough samples. In this project the model had 3,484 No Risk, 616 Diabetic 
and 121 Borderline samples, and the model had trouble telling the 
difference between all three classes even after using SMOTE.
