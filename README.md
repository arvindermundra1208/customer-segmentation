# Unsupervised Clustering for Customer Segmentation

A comprehensive statistical learning project analyzing customer behavior through unsupervised clustering techniques applied to the Online Retail dataset.

## Project Overview

This project undertakes a rigorous statistical analysis of customer behavior through **unsupervised learning techniques** to identify distinct customer segments. The analysis follows a systematic pipeline from raw transactional data to actionable customer segments.

### What This Project Does

The project implements an end-to-end customer segmentation workflow:

1. **Data Engineering**: Transforms raw transactional data into customer-level features using RFM (Recency, Frequency, Monetary) principles and behavioral metrics
2. **Dimensionality Reduction**: Applies Principal Component Analysis (PCA) to reduce feature dimensionality while preserving variance
3. **Clustering Analysis**: Implements and compares multiple clustering algorithms:
   - K-Means clustering
   - Hierarchical Agglomerative Clustering
   - DBSCAN
4. **Evaluation**: Uses statistical metrics to validate segment quality and stability
5. **Validation**: Employs supervised learning to assess segment robustness

## Dataset

**Online Retail Dataset** (UCI Machine Learning Repository)
- **Period**: 2010-2011 transactions from a UK-based online retailer
- **Records**: Transactional-level data spanning multiple customers and products
- **Key Variables**: Invoice ID, Product codes, Quantities, Prices, Timestamps, Customer IDs, Countries

## Methodology

### Feature Engineering
- **RFM Features**: Recency, Frequency, Monetary value per customer
- **Behavioral Metrics**: Purchase patterns, product preferences, spending volatility
- **Temporal Features**: Customer tenure, purchase seasonality

### Dimensionality Reduction
- Principal Component Analysis (PCA) to reduce feature space while maintaining explainability

### Clustering Algorithms
- **K-Means**: Partitioning-based clustering with optimal k selection via elbow method and silhouette analysis
- **Hierarchical Clustering**: Agglomerative approaches with various linkage methods
- **DBSCAN**: Density-based clustering for non-convex cluster detection

### Evaluation Metrics
- Silhouette Score
- Davies-Bouldin Index
- Calinski-Harabasz Index
- Visual inspection via dendrograms and scatter plots

### Validation Strategy
- Supervised learning classification on derived cluster labels
- Cross-validation and performance metrics (accuracy, precision, recall, F1-score)

## 📁 Project Structure

```
customer-segmentation/
├── README.md                          # This file
├── customer segementation.ipynb       # Main analysis notebook
├── STAT654_Final_Report.pdf          # Comprehensive written report
│
├── customer_segementation/            # Analysis artifacts
│   ├── main.tex                       # LaTeX report source
│   ├── references.bib                 # Bibliography
│   └── figures/                       # Generated visualizations
│       ├── fig_*.png                  # 16+ analysis plots
│
└── report/                            # Report generation files
    ├── main.tex
    ├── references.bib
    └── figures/
```

## Key Findings

- Successfully identified distinct customer segments with interpretable characteristics
- RFM-based features proved effective for segmentation
- Clustering algorithms revealed natural groupings without predefined labels
- Segment stability validated through supervised learning classification
- Actionable insights for targeted marketing and customer retention strategies

## Requirements

```
pandas
numpy
matplotlib
seaborn
scikit-learn
scipy
```

## How to Run

1. **Clone the repository**:
   ```bash
   git clone https://github.com/arvindermundra1208/customer-segmentation.git
   cd customer-segmentation
   ```

2. **Install dependencies**:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn scipy
   ```

3. **Download the dataset**:
   - Visit: https://archive.ics.uci.edu/ml/datasets/Online+Retail
   - Download the Excel file and place in the project directory
   - Update the file path in the notebook if needed

4. **Run the analysis**:
   - Open `customer segementation.ipynb` in Jupyter Notebook
   - Execute cells sequentially to reproduce the analysis

## Documentation

- **Jupyter Notebook**: `customer segementation.ipynb` - Complete analysis with code, visualizations, and detailed commentary
- **PDF Report**: `report.pdf` - Comprehensive written report with methodology, results, and conclusions

## Project Status

**COMPLETED** ✓

This is a finished academic project submitted as the final assignment for STAT 654: Statistical Computing with R and Python.

## Course Information

- **Course**: STAT 654 - Statistical Computing with R and Python
- **Type**: Final Project
- **Date Completed**: April 2026
- **Topics**: Unsupervised Learning, Clustering, Statistical Validation, Feature Engineering

## References

See `customer_segementation/references.bib` for complete bibliography including:
- Scikit-learn documentation
- Statistical clustering literature
- RFM analysis methodology
- Customer segmentation best practices

---

**Note**: This project demonstrates practical application of statistical learning theory to real-world business problems, emphasizing both technical rigor and business interpretability.
