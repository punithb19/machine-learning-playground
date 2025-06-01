# Combined Cycle Power Plant: Regression and Predictive Modeling

## Overview
This project analyzes the Combined Cycle Power Plant dataset to predict net hourly electrical energy output (EP) using ambient variables (Temperature, Pressure, Humidity, Vacuum). It applies linear regression, polynomial regression, interaction modeling, and KNN regression to explore and improve predictive performance.

## Dataset
- **Source:** UCI Machine Learning Repository
- **Size:** 9568 rows, 5 columns (4 features + 1 target)[1][16]
- **Features:** 
  - AT: Ambient Temperature (°C)
  - AP: Ambient Pressure (mbar)
  - RH: Relative Humidity (%)
  - V: Exhaust Vacuum (cm Hg)
  - PE: Net hourly electrical energy output (MW) [target]

## Tasks
- Data exploration: scatterplots, summary statistics, outlier analysis
- Simple and multiple linear regression (with significance testing)
- Nonlinear and interaction modeling
- Model improvement using polynomial and interaction terms
- KNN regression (with normalized/raw features, error analysis)
- Comparative analysis of regression models

## Requirements
- Python 3.x
- pandas, numpy, matplotlib, seaborn, scikit-learn, statsmodels

## Usage
1. Clone the repository
2. Install dependencies: `pip install -r requirements.txt`
3. Run the notebook: `jupyter notebook ccpp_regression_analysis.ipynb`

## Results
- Multiple linear regression explains over 90% of the variance in energy output[4][17].
- Model improvement possible with nonlinear and interaction terms.
- KNN regression performance compared to linear models, with error plots for different k values[8][9][14].

## References
- UCI Machine Learning Repository: Combined Cycle Power Plant Data Set
