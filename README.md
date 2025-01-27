# Customer Segmentation - Clustering

This project involves customer segmentation using clustering techniques. The goal is to group customers based on their profile and transaction data to identify patterns and insights.

## Requirements

- Python 3.x
- Libraries:
  - pandas
  - numpy
  - matplotlib
  - seaborn
  - scikit-learn

## Data

The dataset consists of two files:
1. `Customers.csv`: Customer profile data
2. `Transactions.csv`: Customer transaction data

## Steps

1. **Load Data**: The dataset is loaded using `pandas`.
2. **Data Preprocessing**: Missing values are handled by imputing the mean for relevant features.
3. **Clustering**:
   - KMeans clustering is used for customer segmentation.
   - The optimal number of clusters is determined using the **Elbow Method**.
4. **Evaluation**:
   - **Davies-Bouldin Index (DB Index)**: Measures the clustering quality.
   - **Silhouette Score**: Assesses how well each customer fits within their cluster.
5. **Visualization**: PCA is used for dimensionality reduction to plot clusters in 2D.

## Results

- **Number of Clusters**: 4
- **DB Index**: 0.9079
- **Silhouette Score**: 0.3463

## Files

- `customer_segmentation_clustering.py`: Clustering code
- `Clustering.report.pdf`: Report on clustering results
- `Clustering_plots.png`: Visualization of clusters

## How to Run

1. Clone the repository:
