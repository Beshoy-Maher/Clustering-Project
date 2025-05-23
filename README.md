# 🍷 Wine Clustering Project

## 📌 Overview

This project focuses on applying **unsupervised learning** techniques—**K-Means** and various **agglomerative hierarchical clustering methods**—to group different wine samples into clusters based on their chemical attributes. The primary goal is to uncover natural groupings in the data that correspond to the original wine cultivars without using label information.

## 📊 Dataset

- **Source:** [Kaggle - Wine Dataset for Clustering](https://www.kaggle.com/datasets/harrywang/wine-dataset-for-clustering)
- **Attributes:**
  - Alcohol
  - Malic Acid
  - Ash
  - Alcalinity of Ash
  - Magnesium
  - Total Phenols
  - Flavanoids
  - Nonflavanoid Phenols
  - Proanthocyanins
  - Color Intensity
  - Hue
  - OD280/OD315 of Diluted Wines
  - Proline

These attributes represent results from a chemical analysis of wines from three different cultivars in Italy.

## 🧠 Methodology

### 1. **K-Means Clustering**
- Determined optimal number of clusters using **Elbow Method**.
- Optimal `k = 3`.
- R² (WSS/TSS) = **0.447**.

### 2. **Agglomerative Hierarchical Clustering**
- Tested multiple combinations of:
  - **Distance metrics:** Euclidean, Manhattan, Canberra, Minkowski.
  - **Linkage methods:** Ward, Single, Complete, Average, Centroid, Median, McQuitty.
- Evaluated each combination based on:
  - R² statistic.
  - Dendrogram visualizations.
  - Cluster compactness and balance.

#### ✅ Best Combination:
- **Euclidean Distance + Ward’s Method**
- R² = **0.436**

### 🔍 Comparison:
- K-Means and the best hierarchical configuration produced very similar cluster groupings.

## 📈 Evaluation Metric

- **R² Score (WSS/TSS):** Measures proportion of total variance explained by clusters.

## 🛠 Tools & Libraries

- Python (Pandas, NumPy, Scikit-learn, SciPy, Matplotlib, Seaborn)

## 📂 Files

- `wine-clustering.csv` — Raw dataset
- `clustering_analysis.ipynb` — Analysis and visualizations (not uploaded but assumed)
- `Report_Clustering Project.pdf` — Detailed project report

## 🧑‍💻 Authors

- Beshoy M. Botros (900226446)  
- Ahmed M. Monir (900226418)  
- **Course:** Applied Multivariate Analysis  
- **Institution:** The American University in Cairo  
- **Semester:** Spring 2025

## 📬 Contact

For any questions or clarifications, feel free to reach out through the project repository or university portal.
