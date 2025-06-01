# Vertebral Column Pathologies Classification

## Project Overview
Binary classification (Normal vs Abnormal) using biomechanical features:
- Pelvic incidence
- Pelvic tilt  
- Lumbar lordosis
- Sacral slope
- Pelvic radius
- Spondylolisthesis grade

## Dataset
- Source: UCI Machine Learning Repository [1][2]
- 310 instances (100 Normal, 210 Abnormal)
- 6 biomechanical features + class labels

## Methodology
1. Data splitting: 70 Normal + 140 Abnormal training, remainder test
2. KNN implementation with:
   - Euclidean/Manhattan/Chebyshev distances
   - Weighted voting
   - Minkowski parameter tuning
3. Performance metrics:
   - Confusion matrix
   - F1-score
   - Learning curves

## Requirements
- Python 3.8+
- Libraries: NumPy, pandas, scikit-learn, matplotlib

## Usage
1. Clone repository
2. Install dependencies: `pip install -r requirements.txt`
3. Run notebook: `jupyter notebook vertebral_column_knn_classification.ipynb`


