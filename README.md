# Water-Quality-analysis
End-to-end Machine Learning pipeline analyzing CPCB NWMP-2024 water quality across 755 Indian water bodies. Evaluates EDA, K-Means clustering, and tuned ensemble classifiers (Random Forest ~95.4% accuracy) with an interactive web UI for real-time pollution screening.
# 💧 NWMP-2024 Water Quality Analysis & Pollution Profiling

[![Python 3.10+](https://img.shields.io/badge/Python-3.10%2B-blue.svg)](https://www.python.org/)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-1.3%2B-orange.svg)](https://scikit-learn.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Accuracy: 95.4%](https://img.shields.io/badge/Random%20Forest%20Accuracy-95.4%25-brightgreen.svg)]()

An end-to-end Data Science and Machine Learning project analyzing water quality across 755 lakes, ponds, and tanks monitored under the Central Pollution Control Board (CPCB) **National Water Quality Monitoring Programme (NWMP-2024)** across 32 Indian states.

---

## 🌟 Key Features

- **Data Preprocessing & Robust Imputation:** Outlier-resistant median imputation and scaling across 18 physical-chemical water parameters.
- **Exploratory Data Analysis (EDA):** Correlation heatmaps, distribution plots, and class balance analysis across water body types.
- **Unsupervised Learning:** Elbow method & silhouette analysis for **K-Means Clustering** ($K=2\dots7$) and probabilistic **Gaussian Mixture Models (GMM)**.
- **Comprehensive Model Benchmarking:** Side-by-side comparison of **Dummy Baseline, Logistic Regression, Decision Tree, Extra Trees, and Random Forest**.
- **Hyperparameter Optimization:** 5-Fold Stratified Cross-Validation using **GridSearchCV**, achieving **~95.4% accuracy and 0.952 weighted F1-score**.
- **Interactive Web App & Tester:** Standalone UI to search 755 monitored water bodies and test custom samples from any unmonitored river in real-time.

---

## 📊 Model Comparison Overview

| Model | Accuracy (%) | Weighted F1 | Precision | Recall | Training Time (s) |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **Random Forest (Tuned)** | **95.4%** | **0.952** | **0.956** | **0.954** | **0.87s** |
| Extra Trees | 92.8% | 0.928 | 0.931 | 0.928 | 0.42s |
| Decision Tree | 84.1% | 0.840 | 0.843 | 0.841 | 0.04s |
| Logistic Regression | 78.6% | 0.783 | 0.791 | 0.786 | 0.31s |
| Dummy Baseline | 43.2% | 0.261 | 0.187 | 0.432 | 0.02s |
