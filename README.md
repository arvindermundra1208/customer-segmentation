# Customer Segmentation Engine

![Python](https://img.shields.io/badge/Python-3.9%2B-blue) ![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-1.x-orange) ![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

An end-to-end unsupervised machine learning pipeline that segments retail customers into actionable groups using **RFM feature engineering**, **PCA dimensionality reduction**, and three clustering algorithms with rigorous statistical evaluation.

---

## Key Results

- Identified **distinct customer segments** with interpretable business characteristics
- Benchmarked 3 clustering algorithms across 3 evaluation metrics
- Validated segment robustness using supervised learning classification
- Produced **16+ visualizations** documenting the full analytical pipeline
- Actionable insights for targeted marketing and customer retention strategies

---

## Dataset

| Property | Value |
|---|---|
| Source | [UCI Machine Learning Repository — Online Retail](https://archive.ics.uci.edu/ml/datasets/Online+Retail) |
| Period | December 2010 – December 2011 |
| Region | UK-based non-store online retailer |
| Key Variables | Invoice ID, Product codes, Quantities, Prices, Timestamps, Customer IDs |

---

## Pipeline

### 1. Feature Engineering
- **RFM metrics**: Recency (days since last purchase), Frequency (transaction count), Monetary (total spend)
- **Behavioral features**: Purchase patterns, product preferences, spending volatility
- **Temporal features**: Customer tenure, purchase seasonality

### 2. Dimensionality Reduction
- **PCA** applied to reduce feature space and remove multicollinearity before clustering

### 3. Clustering Algorithms

| Algorithm | Description |
|---|---|
| **K-Means** | Centroid-based; optimal K via elbow method and silhouette analysis |
| **Hierarchical Agglomerative** | Bottom-up linkage clustering with dendrogram analysis |
| **DBSCAN** | Density-based; robust to noise and non-convex shapes |

### 4. Evaluation Metrics

| Metric | What It Measures |
|---|---|
| **Silhouette Score** | Cohesion vs. separation of clusters |
| **Davies-Bouldin Index** | Average similarity between each cluster and its nearest neighbor |
| **Calinski-Harabasz Index** | Ratio of between-cluster to within-cluster dispersion |

### 5. Validation
- Supervised classifier trained on cluster labels to confirm segment separability and business utility
- Cross-validation with accuracy, precision, recall, and F1-score metrics

---

## Tech Stack

`Python` · `Pandas` · `NumPy` · `Scikit-learn` · `Matplotlib` · `Seaborn` · `SciPy`

---

## Setup

```bash
pip install pandas numpy matplotlib seaborn scikit-learn scipy
```

Download the dataset from the [UCI repository](https://archive.ics.uci.edu/ml/datasets/Online+Retail), place it in the project root, then open `customer segementation.ipynb` in Jupyter or Google Colab.

---

## Files

| File | Description |
|---|---|
| `customer segementation.ipynb` | Full pipeline: EDA → feature engineering → clustering → evaluation |
| `report.pdf` | Comprehensive written report with methodology and conclusions |
| `customer_segementation.pptx` | Presentation slides summarizing methodology and findings |

---

## Course

**STAT 654 — Statistical Computing with R and Python** · Texas A&M University · Spring 2026

---

## Author

**Arvinder Mundra** · [Portfolio](https://arvindermundraa.github.io/ArvinderMundra/) · [LinkedIn](https://www.linkedin.com/in/arvinder-mundraa) · [GitHub](https://github.com/arvindermundra1208)
