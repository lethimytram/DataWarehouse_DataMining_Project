# Data Mining Project

## Project Overview

This repository presents a data mining project that applies multiple algorithms across different datasets to solve classification, clustering, and association rule mining problems. The work covers preprocessing, model training, evaluation, and comparison among algorithms, using Python.

## Algorithms Applied

The project includes implementations of the following algorithms:

- ID3 (Decision Tree)
- Random Forest
- K-Nearest Neighbors (KNN)
- K-Means Clustering
- Hierarchical Clustering
- Apriori
- FP-Growth

## Datasets and Tasks

### 1. Diabetes Prediction (ID3 and Random Forest)
- **Dataset**: 199 records, 8 features (e.g., gender, age, blood pressure, heart disease, smoking, BMI, glucose level)
- **Target**: `Ket_qua` (diabetes result)
- **Result**:
  - ID3 Accuracy: 72.88% (sensitivity: 55%, specificity: 82.05%)
  - Random Forest Accuracy: 77.97% (sensitivity: 75%, specificity: 79.49%)
- **Insight**: Random Forest outperforms ID3 due to reduced overfitting.

### 2. Online Exam Fraud Detection (KNN)
- **Dataset**: 200 samples, 8 features reflecting interaction behavior
- **Target**: `Fraud` label
- **Method**: KNN with K=5
- **Split**: 70% training, 30% testing

### 3. Lifestyle and Health Clustering (K-Means and Hierarchical)
- **Dataset**: 1000 records, 5 features about personal health and lifestyle
- **K-Means**:
  - Elbow method used to choose K
  - Scatter plot and silhouette scores used for visualization
- **Hierarchical Clustering**:
  - Distance: Euclidean
  - Linkage: Average
  - Result: Hierarchical clustering better reflects natural subgroup structure in data

### 4. Association Rule Mining (Apriori and FP-Growth)
- **Dataset**: 5,000 transaction records from a car care service shop (May 2024 - May 2025)
- **Goal**: Discover frequent itemsets and generate association rules
- **Key Findings**:
  - Car Wash appears in most rules (confidence = 1)
  - Strong association between "Engine Cleaning" and "Interior Vacuuming"
  - Sparse transaction data, suitable for Apriori
- **Comparison**: FP-Growth and Apriori tested on sparse, unbalanced item frequency

## Technologies Used

- Python
- Libraries: `pandas`, `numpy`, `sklearn`, `mlxtend`, `scipy`, `matplotlib`

## Summary

This project demonstrates a comprehensive application of classical data mining techniques on diverse problems. Each algorithm was evaluated using appropriate metrics, and their suitability was discussed based on the data characteristics.

