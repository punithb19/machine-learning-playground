# AReM Time Series Classification

## Overview
This project classifies human activities using the AReM dataset, which contains multivariate time series sensor data from a wireless sensor network. The workflow includes feature extraction, exploratory analysis, and building both binary and multiclass classifiers.

## Dataset
- **Source:** UCI Machine Learning Repository (AReM)
- **Structure:** 7 activity folders, each with multiple files (instances). Each file has 6 time series, each with 480 values[1][2][5].
- **Test/Train Split:** Datasets 1 and 2 in 'bending1' and 'bending2' and datasets 1-3 in other folders are test data; the rest are training data.

## Feature Extraction
- Extracted time-domain features: minimum, maximum, mean, median, standard deviation, 1st quartile, 3rd quartile for each of the 6 time series per instance[2][5].
- Estimated standard deviations and 90% bootstrap confidence intervals for each feature.
- Selected the most important features for classification.

## Modeling
- Binary classification (bending vs. other activities) using logistic regression and L1-penalized logistic regression.
- Multiclass classification using multinomial regression and Naive Bayes (Gaussian and Multinomial priors).
- Used recursive feature elimination and cross-validation (including stratified if needed).
- Evaluated models with confusion matrices, ROC curves, AUC, and accuracy.

## Requirements
- Python 3.x
- numpy, pandas, matplotlib, seaborn, scikit-learn, scipy, statsmodels

## Usage
1. Clone the repository.
2. Install dependencies: `pip install -r requirements.txt`
3. Run the notebook: `jupyter notebook arem_time_series_classification.ipynb`

## Results
- Identified key time-domain features for activity classification.
- Achieved high accuracy in binary and multiclass classification tasks.
- Compared model performance using various metrics and visualizations.

## References
- UCI Machine Learning Repository: AReM Dataset
