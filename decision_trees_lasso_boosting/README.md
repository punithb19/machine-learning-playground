# Acute Inflammations Diagnosis via Decision Trees

## Overview
Binary classification of urinary system diseases using symptom data:
- Diagnosis 1: Bladder inflammation
- Diagnosis 2: Renal pelvis nephritis

## Dataset Features
1. Temperature (35-42°C)
2. Nausea (Yes/No)
3. Lumbar pain (Yes/No)
4. Urine pushing (Yes/No)
5. Micturition pains (Yes/No)
6. Urethra inflammation (Yes/No)[8][10]

## Methodology
- Multi-label decision tree implementation
- Rule extraction using label powerset method
- Cost-complexity pruning with α optimization[3]
- Model interpretation through IF-THEN rules


# Crime Rate Prediction using Regression Models

## Dataset
- Predictors: 128 socio-economic/law enforcement features
- Target: Violent crimes per capita[4][9]
- Key challenges: Missing data, high dimensionality

## Methodology
1. Preprocessing:
   - MICE imputation for missing values
   - Feature selection via CV (√128=11 top features)[6]
   
2. Models:
   - Linear Regression (Baseline)
   - Ridge/LASSO with λ cross-validation[7]
   - Principal Component Regression
   - XGBoost with L1 regularization[6]

3. Evaluation:
   - Test MSE comparison
   - Variable importance analysis
   - Correlation heatmaps

