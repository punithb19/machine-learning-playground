# Anuran Calls: Multi-Label Classification & Clustering

## Overview  
Classify frog species calls using MFCC features via SVMs and evaluate clusters with Hamming metrics. Tasks include:  
- Multi-label classification (Families/Genus/Species)  
- SVM hyperparameter tuning (Gaussian/L1 kernels)  
- Class imbalance handling with SMOTE  
- K-means clustering with automatic k-selection  

## Dataset  
- **Source:** UCI ML Repository (Anuran Calls MFCCs)  
- **Features:** 22 MFCC coefficients per instance  
- **Labels:** 3 hierarchical levels (10 families, 15 genera, 39 species)  
- **Split:** 70% train (stratified sampling)[1][3]  

## Methodology  
### Classification  
- Binary relevance approach (one SVM per label)  
- Kernel tuning:  
  - Gaussian SVM: Optimized σ and C via 10-fold CV[1]  
  - L1-penalized SVM: Feature standardization + penalty tuning  
- Evaluation:  
  - Exact Match (%)  
  - Hamming Loss/Score[1][3]  
  - Multi-label ROC/AUC (micro-averaged)  

### Clustering  
- K-means with Silhouette-based k selection (1-50)  
- Majority label assignment per cluster  
- Hamming distance analysis vs true labels[3]  

## Requirements  
- Python 3.8+  
- Libraries: scikit-learn, imbalanced-learn, scikit-multilearn  

## References  
1. UCI Anuran Calls (MFCCs) Dataset  
2. Scikit-multilearn Documentation  
