# Data Warehouse & Data Mining Project

## Overview

This repository contains a comprehensive analytics project that integrates two key components:

1. **Data Warehouse** – applying ETL, OLAP, MDX, and dashboard design for nutrition data analysis.
2. **Data Mining** – implementing machine learning and data mining techniques for classification, clustering, and association tasks.

The project demonstrates the ability to extract insights from both structured warehouse data and raw datasets using analytical and predictive approaches.

## Technologies Used

- Python (`pandas`, `numpy`, `scikit-learn`, `mlxtend`, `matplotlib`)
- Power BI (dashboard creation)
- MDX for OLAP querying

---
## Part 1: Data Warehouse – Nutrition Analytics

### Project Title

**Daily Food Nutrition Analysis to Support a Healthy Lifestyle**

### Dataset Description

- **Name**: `daily_food_nutrition`
- **Size**: 10,000 food intake records from 1,000 unique users
- **Features**: Food name, calories, sugar, fiber, protein, user ID, meal time
- **Goal**: Analyze dietary behavior and provide recommendations for healthier lifestyles

### ETL Process

- **Data Preparation**:
  - Cleaned and transformed raw data
  - Handled missing values and standardization
- **Data Modeling**:
  - Designed and implemented a **Star Schema**
  - Built fact and dimension tables for food, user, and nutrient data

### OLAP Operations

- **Drill Down / Roll Up**: Navigate between high-level summaries and specific meal types or nutrient details
- **Slice / Dice**: Analyze dietary patterns by age group, food category, or individual users

### MDX Queries

Executed multidimensional MDX queries to extract:
- Average calorie intake per user
- Top sources of sugar across age groups
- Nutrient breakdown by meal type (e.g., breakfast vs. lunch)

### Dashboard (Power BI)

A summary dashboard was built using Power BI, featuring:
- Total daily nutrient intake by user
- High-sugar food items by frequency
- Visual recommendations for increasing fiber and reducing sugar

#### Key Insights:
- Users aged 20–21 had the highest average calorie intake (~1169 kcal/day)
- Top sugar sources included: milk tea, coffee, fruit juices
- Suggested improvements:
  - Reduce sugar (beverages)
  - Increase fiber and protein in main meals
  - Move toward the 2000 kcal/day target

---

## Part 2: Data Mining

### Algorithms Implemented

- ID3 (Decision Tree)
- Random Forest
- K-Nearest Neighbors (KNN)
- K-Means Clustering
- Hierarchical Clustering
- Apriori
- FP-Growth

### Tasks and Datasets

#### 1. Diabetes Prediction
- **Dataset**: 199 records, 8 features (e.g., age, blood pressure, BMI)
- **Target**: `Ket_qua` (diabetes outcome)
- **Results**:
  - ID3 Accuracy: 72.88%
  - Random Forest Accuracy: 77.97%
- **Conclusion**: Random Forest outperforms ID3 by mitigating overfitting

#### 2. Online Exam Fraud Detection
- **Dataset**: 200 samples representing online exam behavior
- **Target**: `Fraud`
- **Method**: KNN with K=5

#### 3. Health Clustering
- **Dataset**: 1,000 records on lifestyle behavior
- **Clustering**:
  - K-Means (Elbow method for K selection)
  - Hierarchical (Average linkage, Euclidean distance)
- **Conclusion**: Hierarchical clustering suited the naturally stratified health data

#### 4. Car Service Association Rules
- **Dataset**: 5,000 transactions from a car service shop
- **Goal**: Find frequent itemsets and derive association rules
- **Result**:
  - Strong rules: Car Wash → other services (confidence = 1)
  - FP-Growth and Apriori were compared for efficiency

---

## Summary

This project showcases an end-to-end data analytics pipeline, from data warehousing to mining. It applies structured multidimensional analysis and predictive modeling to extract meaningful insights for real-world decision-making in both health and behavioral domains.
