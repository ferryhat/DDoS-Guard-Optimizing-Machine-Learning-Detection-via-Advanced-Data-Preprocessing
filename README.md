# DDoS-Guard-Optimizing-Machine-Learning-Detection-via-Advanced-Data-Preprocessing
This project evaluates how data preprocessing improves machine learning detection of DDoS attacks using the CIC-DDoS2019 dataset (50M+ records). A four-stage framework enhances accuracy and efficiency, comparing Random Forest, XGBoost, k-NN, Naïve Bayes, and SVM to achieve near-perfect detection in complex networks.
DDoS Detection Performance via Machine Learning
🚀 Overview
In a landscape of increasingly frequent and sophisticated DDoS threats, automated detection is a critical cybersecurity challenge
. This repository contains the implementation of a high-performance detection system that analyzes the CIC-DDoS2019 dataset
.
The core contribution of this work is the comparative analysis of four distinct preprocessing versions, ranging from raw data handling to advanced statistical feature selection, to determine the optimal pipeline for real-time intrusion detection
.
📊 Key Results
Peak Accuracy: Achieved 99.99% accuracy using Random Forest and XGBoost
.
Efficiency: Reduced feature dimensionality by 88% (from 88 to 10 features), allowing XGBoost to train in just 61.57 seconds [21, 301, previous response].
Robustness: Boosted Naïve Bayes accuracy from 45% (baseline) to 99.80% through optimized class balancing and cleaning
.
🛠 Preprocessing Pipeline
The project evaluates four specific configurations to measure the impact on model performance:
Version 1 (Raw): Minimal processing with binary encoding and handling of infinite values
.
Version 2 (Standard): Basic cleaning, normalization, and class balancing using SMOTE
.
Version 3 (Advanced): Dimensionality reduction via Pearson correlation and balancing with ADASYN
.
Version 4 (Profound): Advanced feature selection based on the slope of regression lines for highly correlated pairs, minimizing multi-collinearity
.
🧠 Models Implemented
Random Forest: Best overall stability and performance
.
XGBoost (Extreme Gradient Boosting): Highly efficient for massive datasets
.
k-Nearest Neighbors (k-NN): Effective but computationally expensive for large scales
.
Support Vector Machine (SVM): High sensitivity but requires significant optimization
.
Naïve Bayes: Optimized for low-resource environments
.
💻 Tech Stack
Language: Python
.
Libraries: Pandas, NumPy, Scikit-learn, XGBoost, Matplotlib, Seaborn
.
Environment: Google Colab Pro+ with high-RAM (334GB) for handling 22GB CSV files
