# DDoS-Guard-Optimizing-Machine-Learning-Detection-via-Advanced-Data-Preprocessing
This project evaluates how data preprocessing improves machine learning detection of DDoS attacks using the CIC-DDoS2019 dataset (50M+ records). A four-stage framework enhances accuracy and efficiency, comparing Random Forest, XGBoost, k-NN, Naïve Bayes, and SVM to achieve near-perfect detection in complex networks.
# DDoS-Guard: Optimizing ML Detection via Advanced Data Preprocessing

## 📌 Project Overview
This repository contains the research, implementation, and performance evaluation of my Master’s graduation project in **Computer Systems and Networks** at the University of Saad Dahlab Blida 1.

The project investigates how iterative **data preprocessing strategies**—including specialized cleaning, dimensionality reduction, and class balancing—impact the efficacy of Machine Learning models in detecting **Distributed Denial of Service (DDoS)** attacks. Using the massive **CIC-DDoS2019** dataset (50 million+ records), we developed a framework that achieves near-perfect detection while drastically optimizing computational speed.

## 📊 Key Performance Highlights
*   **Peak Accuracy:** Achieved **99.99% accuracy** and **99.95% recall** using Random Forest (Version 4).
*   **Efficiency Gain:** Reduced the feature set by **88%** (from 88 down to 10 key features) using statistical slope analysis.
*   **High-Speed Processing:** Optimized XGBoost to train on millions of records in just **61.57 seconds** without sacrificing reliability.
*   **Model Robustness:** Boosted Naïve Bayes accuracy from a literature baseline of **45%** to **99.80%** through optimized class balancing.

## 🧪 The 4-Stage Preprocessing Framework
We implemented four distinct configurations to measure the impact of data preparation on performance:

1.  **Version 1 (Raw):** Minimal processing; binary encoding and handling of infinite values.
2.  **Version 2 (Standard):** Basic cleaning, Min-Max normalization, and class balancing via **SMOTE**.
3.  **Version 3 (Advanced):** Redundancy elimination via **Pearson correlation** and balancing via **ADASYN**.
4.  **Version 4 (Profound):** Advanced feature selection based on **regression line slopes** to eliminate multi-collinearity, retaining only the 10 most informative features.

## 🤖 Models Evaluated
*   **Random Forest:** Best overall stability and generalization across all versions.
*   **XGBoost:** Most efficient for massive-scale datasets and high-speed training.
*   **k-Nearest Neighbors (k-NN):** High accuracy but computationally expensive for large traffic volumes.
*   **Support Vector Machine (SVM):** High sensitivity after specialized normalization.
*   **Naïve Bayes:** Optimized for low-resource environments.

## 💻 Tech Stack & Infrastructure
*   **Language:** Python
*   **Libraries:** Pandas, NumPy, Scikit-learn, XGBoost, Matplotlib, Seaborn
*   **Environment:** Google Colab Pro+ with high-RAM (334GB) and TPU support to handle the 22GB dataset.
*   **Storage:** Google Cloud Storage for large-scale CSV management.

## 📂 Repository Structure
*   `/notebooks`: Step-by-step Jupyter notebooks for EDA and Preprocessing Versions 1–4.
*   `/scalers`: Saved `.pkl` files for the optimized MinMaxScaler configurations.
*   `/results`: Visualizations of Confusion Matrices, Learning Curves, and AUC-ROC comparisons.
*   `requirements.txt`: Python dependencies.

## 🎓 Acknowledgments
This project was realized as a graduation thesis under the supervision of **Mr. Mohamed Benyahia**.
**Authors:** Hattou Feriel & Mekki Nadjet.
