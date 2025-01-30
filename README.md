# Clustering Algorithms Comparative Analysis

## Overview
This repository contains Python code to perform various clustering techniques on a given dataset. The purpose of this analysis is to apply different clustering algorithms, visualize their results, and evaluate their performance. This will aid in selecting the most suitable clustering method based on the characteristics of the data and the specific problem requirements.

## Objective
The main objective is to compare multiple clustering algorithms, analyze their performance, and interpret the results for practical decision-making. This analysis can be applied in real-world scenarios such as customer segmentation, pattern recognition, and anomaly detection.

## Clustering Algorithms Used

### 1. **K-Means Clustering**
- Partitions the dataset into a predefined number of clusters (e.g., 6).
- Assigns each data point to the nearest cluster centroid.
- Assumes clusters are spherical and of similar sizes.

### 2. **Affinity Propagation**
- Uses exemplar-based clustering where data points act as representatives of clusters.
- Works by passing messages between points to determine exemplars and form clusters.
- Computationally expensive and not ideal for large datasets.

### 3. **Mean Shift**
- Identifies dense regions of data points without requiring a predefined number of clusters.
- Relies on a critical `bandwidth` parameter to define region size.

### 4. **Spectral Clustering**
- Leverages connectivity of data points by transforming data into a lower-dimensional space.
- Useful for non-linearly separable data.
- Computationally intensive and sensitive to the number of clusters.

### 5. **Agglomerative Clustering (Hierarchical)**
- Follows a bottom-up approach, merging data points into clusters based on proximity.
- Visualized using a dendrogram to show cluster merging.
- Ward linkage minimizes variance within clusters.

### 6. **DBSCAN (Density-Based Spatial Clustering of Applications with Noise)**
- Finds arbitrarily shaped clusters and handles noise (outliers).
- Requires two parameters: `eps` (maximum distance for neighbors) and `min_samples` (minimum points to form a cluster).

### 7. **HDBSCAN (Hierarchical DBSCAN)**
- Extends DBSCAN using hierarchical clustering.
- Robust to varying cluster densities and effective at handling outliers.

## Key Observations

| Algorithm            | Strengths                                      | Weaknesses                                  |
|----------------------|-----------------------------------------------|---------------------------------------------|
| **K-Means**         | Fast and effective for spherical clusters.    | Struggles with irregularly shaped clusters. |
| **Affinity Propagation** | Handles varying cluster sizes.               | Slow and computationally expensive.         |
| **Mean Shift**       | No need to specify cluster count.             | Sensitive to `bandwidth`.                   |
| **Spectral Clustering** | Effective for complex structures.            | Computationally intensive for large data.   |
| **Agglomerative**    | Suitable for hierarchical data.               | Slower for large datasets.                  |
| **DBSCAN**           | Finds arbitrary shapes and handles noise.     | Sensitive to `eps` and `min_samples`.       |
| **HDBSCAN**          | Robust to varying densities and noise.        | Slightly more complex to tune.              |

## Dataset

1. **Synthetic Dataset**: `cluster_data.npy` for testing clustering algorithms.
2. **Real-World Dataset**: `shopping-data.csv` for Agglomerative Clustering, focusing on customer shopping behaviors.

## How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/Clustering-Algorithm-Analysis.git
   ```

2. Install the required libraries:
   ```bash
   pip install numpy matplotlib seaborn scikit-learn hdbscan
   ```

3. Run the script:
   - Ensure `cluster_data.npy` and `shopping-data.csv` are in the appropriate directories.
   - Replace `cluster_data.npy` with your own dataset if needed.

4. Visualize results for each clustering algorithm.

## Conclusion
This repository provides a comparative analysis of multiple clustering algorithms. By running the code, you can evaluate how each algorithm performs on different datasets and gain insights into their strengths and weaknesses. The analysis is designed to help you choose the most appropriate algorithm for tasks like customer segmentation, anomaly detection, and pattern recognition.
