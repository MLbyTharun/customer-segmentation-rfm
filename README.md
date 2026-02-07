# 🛒 Customer Segmentation with RFM Analysis

## 📌 Overview
This project focuses on **customer segmentation** using **RFM (Recency, Frequency, Monetary) analysis** applied to an online retail dataset.  
The goal is to identify distinct customer groups based on purchasing behavior, enabling businesses to design targeted marketing strategies, improve customer retention, and maximize revenue.

By combining **data preprocessing, feature engineering, dimensionality reduction, and clustering algorithms**, the project demonstrates how data science can uncover actionable business insights.

---

## 🎯 Objectives
- Clean and preprocess raw retail transaction data.
- Engineer RFM features to quantify customer behavior.
- Apply clustering algorithms (**KMeans** and **Gaussian Mixture Models**) to group customers.
- Evaluate clustering performance using metrics like **Silhouette Score** and **Davies-Bouldin Index**.
- Visualize customer segments in reduced dimensions using **PCA**.
- Provide business interpretations of each cluster.

---

## 🚀 Features
- **Data Cleaning**:
  - Removed cancelled orders (InvoiceNo starting with "C").
  - Filtered out negative or zero quantities and prices.
  - Handled missing values in `CustomerID`.
- **Feature Engineering**:
  - Recency: Days since last purchase.
  - Frequency: Number of unique invoices.
  - Monetary: Total spending.
  - Added `TotalPrice` column for transaction-level spending.
- **Transformation & Scaling**:
  - Log transformation to reduce skewness.
  - Standardization using `StandardScaler`.
- **Dimensionality Reduction**:
  - Principal Component Analysis (PCA) for visualization.
- **Clustering**:
  - KMeans clustering with Elbow Method and Silhouette analysis.
  - Gaussian Mixture Models (GMM) for probabilistic clustering.
- **Evaluation**:
  - Compared KMeans vs GMM using Silhouette Score and Davies-Bouldin Index.
- **Visualization**:
  - PCA scatter plots of clusters.
  - Boxplots of RFM distributions by cluster.
  - Cluster centers projected in PCA space.

---

## 🛠️ Installation
Clone the repository and install dependencies:

```bash
git clone https://github.com/your-username/customer-segmentation.git
cd customer-segmentation
pip install -r requirements.txt
