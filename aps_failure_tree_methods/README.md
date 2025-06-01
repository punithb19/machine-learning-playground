# APS Failure Prediction using Tree-Based Methods

## Objective  
Predict air pressure system failures in Scania trucks using sensor data, addressing high dimensionality and extreme class imbalance.

## Dataset  
- **Source:** UCI ML Repository (APS Failure)  
- **Training:** 60k instances (1k failures)  
- **Test:** 16k instances  
- **Features:** 170 sensor measurements (all numeric)  

## Methodology  
1. **Data Preparation**  
   - MICE imputation for missing values  
   - Feature selection: Top 13 features by CV (√170 ≈13)  
   - Correlation matrix analysis  

2. **Modeling Techniques**  
   - **Random Forest:**  
     - Baseline (uncompensated) vs. class weight adjustment  
     - OOB error vs test error comparison  
   - **XGBoost with L1 Regularization:**  
     - Node splits using penalized logistic regression  
     - 10-fold cross-validation for α tuning  
   - **SMOTE:** Synthetic minority oversampling  

3. **Evaluation Metrics**  
   - AUC-ROC curves  
   - Confusion matrices (precision/recall tradeoff)  
   - Misclassification costs

## Requirements  
- Python 3.8+  
- Libraries: XGBoost, imbalanced-learn, missingpy, scikit-learn  

