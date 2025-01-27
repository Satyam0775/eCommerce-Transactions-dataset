# Customer Segmentation - Clustering

This project focuses on customer segmentation using clustering techniques. The goal is to group customers based on their profile and transaction data to identify patterns and insights that can help businesses understand their customers better.

## Project Overview

### Objective:
- Perform customer segmentation using both **profile** and **transaction** data.
- Apply clustering algorithms to form distinct customer groups based on their behaviors.

### Clustering Technique:
- **KMeans** clustering algorithm was chosen for segmentation.
- The number of clusters was determined using the **Elbow Method** and validated with **Silhouette Score** and **Davies-Bouldin Index (DB Index)**.

## Datasets

The project uses two datasets:
1. **Customers.csv**: Contains customer profile information.
   - Columns: `CustomerID`, `Region`, `TotalSpending`, `NumTransactions`, `AvgTransactionValue`
2. **Transactions.csv**: Contains customer transaction details.

The `Customers.csv` file contains information like total spending, number of transactions, and the average transaction value.

## Steps

1. **Load and Preprocess Data**:
   - Read the data from `Customers.csv` and `Transactions.csv`.
   - Handle missing values by imputing them with the column mean.
   
2. **Clustering with KMeans**:
   - Use KMeans clustering to perform customer segmentation.
   - Optimal number of clusters determined by **Elbow Method**.

3. **Clustering Evaluation**:
   - **Davies-Bouldin Index**: Measures the compactness and separation of the clusters.
   - **Silhouette Score**: Assesses how well each customer fits into their assigned cluster.

4. **Dimensionality Reduction**:
   - **PCA (Principal Component Analysis)** is applied to reduce the data to 2D for visualization.

5. **Visualization**:
   - Visualize the clusters using a 2D scatter plot to show the customer segments.

## Results

- **Number of Clusters**: 4 (Optimal clusters as determined by the Elbow Method)
- **Davies-Bouldin Index (DB Index)**: 0.9079 (Lower value indicates better clustering)
- **Silhouette Score**: 0.3463 (Higher value indicates better-defined clusters)

## Files

- **customer_segmentation_clustering.py**: Python script containing the clustering code.
- **Clustering.report.pdf**: A detailed report on clustering results, metrics, and analysis.
- **Clustering_plots.png**: Visualization of the customer clusters after applying PCA for dimensionality reduction.

## How to Run the Code

1. **Clone the Repository**:
