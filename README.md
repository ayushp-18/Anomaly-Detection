# Anomaly Detection in Credit Card Transactions

## Brief One Line Summary
Unsupervised machine learning models applied to detect fraudulent transactions in a highly imbalanced dataset of 284,807 credit card records.

## Overview
Fraud detection in financial transactions is a critical problem as fraudulent activities cause significant losses. The challenge lies in detecting rare fraud events in highly imbalanced datasets. This project implements anomaly detection algorithms to identify fraudulent transactions effectively.

## Problem Statement
- Identify fraudulent transactions in credit card data.  
- Work with an extremely imbalanced dataset (0.172% fraud cases).  
- Compare multiple anomaly detection models to determine the most effective approach.  

## Dataset
- Source: [Kaggle – Credit Card Fraud Detection Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)  
- Records: 284,807  
- Fraud cases: 492 (0.172%)  
- Features: 30 (V1–V28 are PCA-transformed, plus Time and Amount).  

## Tools and Technologies
- Python  
- Pandas, NumPy, Matplotlib, Seaborn  
- Scikit-learn  

## Methods
- Isolation Forest  
- Local Outlier Factor (LOF)  
- One-Class SVM  

## Key Insights
- Fraud cases are extremely rare, requiring anomaly detection methods instead of standard classification.  
- Isolation Forest consistently outperformed LOF and One-Class SVM in both accuracy and scalability.  
- Precision and recall are critical metrics alongside accuracy in fraud detection problems.  



## How to Run
1. Clone this repository  
   ```bash
   git clone https://github.com/your-username/Anomaly-Detection.git
   cd Anomaly-Detection

2. Install dependencies 
   ```bash
   pip install -r requirements.txt

3. Run the notebook
    ```bash
    jupyter notebook "Anamoly Detection.ipynb"



## Results & Conclusion

Isolation Forest: 99.74% accuracy (best performing model).

Local Outlier Factor: Reliable but slightly less accurate.

One-Class SVM: Struggled with computation on large dataset.

Conclusion: Isolation Forest is the most effective anomaly detection method for fraud detection in highly imbalanced datasets.

## Future Work

Explore deep learning methods such as Autoencoders and GANs for anomaly detection.

Improve accuracy by improving the sample size.


