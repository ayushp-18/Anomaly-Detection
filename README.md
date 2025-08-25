# Anomaly Detection in Credit Card Transactions

## Overview
This project applies unsupervised machine learning models to detect fraudulent credit card transactions in a highly imbalanced dataset. The dataset contains 284,807 transactions, of which only 0.172% are fraud cases, making it an excellent benchmark for anomaly detection techniques.

## Objective
- Detect fraudulent transactions using anomaly detection algorithms.  
- Handle highly imbalanced data effectively.  
- Compare model performance based on accuracy and reliability.  

## Dataset
- Source: [Kaggle – Credit Card Fraud Detection Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)  
- Records: 284,807  
- Fraud cases: 492 (0.172%)  
- Features: 30 (V1–V28 are PCA-transformed, Time, and Amount).  

## Technologies Used
- Python  
- Pandas, NumPy, Matplotlib, Seaborn  
- Scikit-learn  

## Methods Implemented
- Isolation Forest  
- Local Outlier Factor (LOF)  
- One-Class SVM  

## Results
- Isolation Forest: 99.74% accuracy (best performing model)  
- Local Outlier Factor: Reliable but slightly lower accuracy  
- One-Class SVM: Struggled with large dataset size  

Isolation Forest proved to be the most effective model for rare-event fraud detection.

## Key Insights
- Anomaly detection methods can effectively identify rare fraud cases in highly imbalanced data.  
- Ensemble tree-based methods like Isolation Forest outperform distance/kernel-based methods on large datasets.  
- Useful for financial fraud detection systems where false positives must be minimized.  

## How to Run
1. Clone this repository  
   ```bash
   git clone https://github.com/your-username/Anomaly-Detection.git
   cd Anomaly-Detection
