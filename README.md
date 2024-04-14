# K-Means Clustering Algorithm
This program implements the K-means clustering algorithm using OpenMP. 
The k-means algorithm is a popular clustering technique used in data mining and machine learning. It's used to partition a dataset into groups (clusters) based on similarities in the data points' features.

##How it works
Initialization: Choose the number of clusters (k) you want to create and randomly initialize k cluster centroids. These centroids represent the centers of the clusters.

Assign Data Points to Clusters: For each data point in the dataset, calculate its distance to each cluster centroid. Assign the data point to the cluster whose centroid is closest (usually based on Euclidean distance).

Update Cluster Centroids: Once all data points are assigned to clusters, calculate the mean (centroid) of the data points in each cluster. Move the cluster centroid to this mean position.

Repeat: Repeat steps 2 and 3 until convergence. Convergence occurs when the cluster assignments no longer change significantly, or when a maximum number of iterations is reached.

Final Clustering: Once the algorithm converges, each data point belongs to the cluster corresponding to the nearest centroid.

