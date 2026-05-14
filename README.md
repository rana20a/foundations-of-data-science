# 📊 Foundations of Data Science — Lab Portfolio
### CIS 6211 | King Khalid University

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter&logoColor=white)
![sklearn](https://img.shields.io/badge/scikit--learn-ML-green?logo=scikit-learn&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-Pandas-lightblue?logo=numpy&logoColor=white)

> **Course:** CIS 6211 – Foundations of Data Science — King Khalid University  
> **Author:** Rana Sultan Alhinidy

---

## 📋 Overview

A collection of 7 hands-on labs covering the full data science pipeline — from mathematical foundations and data cleaning, through regression modeling and model evaluation. Each lab includes working Python code with visualizations and written analysis.

---

## 🗂️ Lab Index

| Lab | Topic | Key Concepts | Dataset |
|---|---|---|---|
| [Lab 1](#lab-1) | Mathematical Preliminaries | PDF/CDF, Correlation, PCA, Autocorrelation | Synthetic |
| [Lab 2](#lab-2) | Data Collection & Integration | CSV + JSON merge, API data, Schema inspection | Airbnb NYC 2019, OpenWeatherMap |
| [Lab 3](#lab-3) | Data Cleaning & Preprocessing | Missing values, Outlier detection, Winsorization | Adult Income |
| [Lab 4](#lab-4) | Mathematical Models | Confusion matrix, ROC Curve, TPR/FPR | Height/Weight |
| [Lab 5](#lab-5) | Linear Algebra | 3D Vectors, Unit vectors, PCA projection | Synthetic |
| [Lab 6](#lab-6) | Linear & Logistic Regression | Gradient descent, Cost functions, Decision boundary | Height/Weight |
| [Lab 7](#lab-7) | Visualizing Model Performance | AUC-ROC, Precision-Recall, Learning curves, Feature importance | Breast Cancer (sklearn) |

---

## 🔬 Lab Highlights

### Lab 1
**Mathematical Preliminaries**

Explored core statistical concepts through visualization:
- Probability distributions (PDF and CDF) using dice simulation
- Pearson vs Spearman correlation — when each fails
- R² interpretation and its relationship to Pearson coefficient
- Autocorrelation to detect weekly seasonality in website traffic
- Log-Normal distributions and scale choice

---

### Lab 2
**Data Collection & Integration**

Integrated two real-world datasets from different formats:
- Loaded the **Airbnb NYC 2019** dataset (48,000+ listings) from CSV
- Fetched **New York weather data** from OpenWeatherMap API (JSON)
- Performed schema inspection and left-join merge on city key
- Documented integration challenges (structure mismatch, single-snapshot weather)

---

### Lab 3
**Data Cleaning & Preprocessing**

Cleaned the **UCI Adult Income** dataset (30,000+ rows):
- Identified missing values encoded as `?` in workclass, occupation, native_country
- Applied row-dropping strategy (justified by large dataset size)
- Detected extreme right-skew in `capital_gain` via box plot
- Applied **Winsorization (99th percentile capping)** to handle outliers

---

### Lab 4
**Mathematical Models**

Built an ROC curve from scratch using height/weight data:
- Visualized confusion matrix regions (TP, TN, FP, FN) on overlapping distributions
- Manually computed TPR and FPR across all thresholds
- Demonstrated how threshold choice affects the precision/recall tradeoff

---

### Lab 5
**Linear Algebra**

Visualized vector concepts in 3D space:
- Plotted random 3D points and their vector representations
- Normalized vectors to unit length (demonstrated cosine similarity principle)
- Applied **PCA** to 2D data and visualized perpendicular projection

---

### Lab 6
**Linear & Logistic Regression**

Covered the full regression pipeline:
- Simple linear regression with residual analysis
- Effect of outliers on regression line
- Linear vs quadratic fit (underfitting demonstration)
- Z-score normalization before regression
- MSE cost function visualization (U-shaped curve)
- 3D convex cost surface and non-convex surface (local minima problem)
- Sigmoid function and logistic regression for gender classification

---

### Lab 7
**Visualizing Model Performance**

Comprehensive model evaluation on the **Breast Cancer** dataset:

| Metric | Logistic Regression | Random Forest |
|---|---|---|
| Accuracy | **97.7%** | 97.1% |
| AUC-ROC | **0.998** | 0.997 |
| Avg Precision | **0.999** | — |

- Confusion matrix analysis (TP=106, TN=61, FP=2, FN=2)
- ROC and Precision-Recall curve comparison
- Learning curves — detected overfitting in Decision Tree (max_depth=10)
- Feature importance: **mean concave points** ranked #1
- 5-model comparison: Logistic Regression, Random Forest, KNN, SVM, Naive Bayes

---

## 📁 Repository Structure

```
foundations-of-data-science/
│
├── README.md
│
├── notebooks/
│   ├── Lab01_Mathematical_Preliminaries.ipynb
│   ├── Lab02_Data_Collection_Integration.ipynb
│   ├── Lab03_Data_Cleaning.ipynb
│   ├── Lab04_Mathematical_Models.ipynb
│   ├── Lab05_Linear_Algebra.ipynb
│   ├── Lab06_Linear_Logistic_Regression.ipynb
│   └── Lab07_Visualizing_Model_Performance.ipynb
│
└── data/
    ├── AB_NYC_2019.csv          ← Airbnb NYC 2019 listings
    ├── weather_sample.json      ← OpenWeatherMap API sample
    ├── adult.data               ← UCI Adult Income dataset
    ├── adult.names              ← Column descriptions
    └── weight.xls               ← Height/Weight dataset
```

---

## 🛠️ Tech Stack

| Library | Purpose |
|---|---|
| `numpy` | Numerical operations, array math |
| `pandas` | Data loading, cleaning, merging |
| `matplotlib` | Plotting and visualization |
| `seaborn` | Statistical visualizations |
| `scipy.stats` | Correlation coefficients, statistical functions |
| `sklearn` | PCA, Logistic Regression, Random Forest, metrics |

---

## 🚀 Getting Started

```bash
# Clone the repository
git clone https://github.com/YOUR_USERNAME/foundations-of-data-science.git
cd foundations-of-data-science

# Install dependencies
pip install numpy pandas matplotlib seaborn scikit-learn scipy openpyxl

# Launch Jupyter
jupyter notebook notebooks/
```

---

## 🎓 Academic Context

**University:** King Khalid University  
**Course:** CIS 6211 – Foundations of Data Science  

Labs cover: probability & statistics → data collection → data cleaning → mathematical models → linear algebra → regression → model evaluation

---

## 📄 License

Developed for academic purposes at King Khalid University.
