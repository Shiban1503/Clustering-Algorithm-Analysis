# Clustering-Algorithm
Comparing SKLEARN Clustering Algorithms

#Overview
This project provides a comprehensive comparative analysis of various clustering algorithms using Python and machine learning libraries. The analysis explores different clustering techniques, their characteristics, and performance on a given dataset.

The project implements and analyzes six sophisticated clustering algorithms:

**#K-Means Clustering**
Core Concept: Partitioning method dividing data into k-number of clusters

**Key Parameters:**
Cluster Count: 6
Optimal for large, well-separated datasets

**Limitations:**
Assumes spherical clusters
Prone to forcing points into clusters

**#Affinity Propagation**
Core Concept: Exemplar-based clustering without predefined cluster count

**Key Parameters:**
Preference: -6.0
Damping: 0.95

**Challenges:**
Computationally expensive
Inefficient for large datasets




Mean Shift Clustering

Core Concept: Density-based clustering adapting to non-linear data structures
Key Parameters:

Bandwidth: 0.19


Characteristics:

Flexible cluster shape detection
Sensitive to bandwidth selection




Spectral Clustering

Core Concept: Graph-based clustering using eigenvalue decomposition
Key Parameters:

Cluster Count: 4


Strengths:

Handles non-convex cluster shapes
Effective for interconnected data




Agglomerative Clustering

Core Concept: Hierarchical bottom-up clustering approach
Key Parameters:

Cluster Count: 5
Linkage Method: Ward


Visualization: Dendrogram representation


HDBSCAN

Core Concept: Advanced density-based spatial clustering
Key Parameters:

Minimum Cluster Size: 17


Strengths:

Handles varying cluster densities
Robust to noise
Most reliable clustering method
