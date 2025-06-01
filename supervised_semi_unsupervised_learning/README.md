# Supervised, Semi-Supervised, and Unsupervised Learning

## Overview

This repository explores supervised, semi-supervised, unsupervised, and active learning approaches for classification using two real-world datasets:

- **Breast Cancer Wisconsin (Diagnostic)**
- **Banknote Authentication**

We compare how various learning paradigms perform, especially when labeled data is limited.

---

## Datasets

- **Breast Cancer Wisconsin (Diagnostic)**
  - 30 numerical features from digitized images of breast tissue
  - Binary labels: Malignant or Benign
  - [UCI Dataset Link](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+(Diagnostic))

- **Banknote Authentication**
  - 4 numerical features from banknote images
  - Binary labels: Authentic or Forged
  - [UCI Dataset Link](https://archive.ics.uci.edu/ml/datasets/banknote+authentication)

---

## Methods

- **Supervised Learning**
  - Models: SVM, Logistic Regression, Decision Tree
  - Metrics: Accuracy, Precision, Recall, F1-score, Confusion Matrix

- **Semi-Supervised Learning**
  - Techniques: Self-training, Label Propagation
  - Uses small labeled set + large unlabeled set

- **Unsupervised Learning**
  - Algorithms: K-Means, Hierarchical Clustering
  - Metrics: Silhouette Score, Adjusted Rand Index

- **Active Learning**
  - Iteratively selects most informative samples for labeling
  - Compared with random sampling


