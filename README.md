# K-Means Clustering Algorithm

This program implements the K-means clustering algorithm using OpenMP. The k-means algorithm is a popular clustering technique used in data mining and machine learning. It's used to partition a dataset into groups (clusters) based on similarities in the data points' features.

## Algorithm

The K-means algorithm follows these steps:

Initialization: Choose the number of clusters (k) you want to create and randomly initialize k cluster centroids. These centroids represent the centers of the clusters.

Assign Data Points to Clusters: For each data point in the dataset, calculate its distance to each cluster centroid. Assign the data point to the cluster whose centroid is closest (usually based on Euclidean distance).

Update Cluster Centroids: Once all data points are assigned to clusters, calculate the mean (centroid) of the data points in each cluster. Move the cluster centroid to this mean position.

Repeat: Repeat steps 2 and 3 until convergence. Convergence occurs when the cluster assignments no longer change significantly, or when a maximum number of iterations is reached.

Final Clustering: Once the algorithm converges, each data point belongs to the cluster corresponding to the nearest centroid.

## Application 

The K-means algorithm finds applications in various domains, including:

- **Recommendation Systems**: Segmenting users or items based on preferences, ratings, or purchase history to generate personalized recommendations for products, movies, music, or other content
- **Document Clustering**:  Organizing large document collections into clusters based on their content similarity, facilitating tasks such as information retrieval, document summarization, and topic modeling.
- **Image Segmentation**:  Grouping pixels in an image into distinct regions based on color or texture similarity, useful in computer vision tasks like object detection and image compression.
- **Anomaly Detection**: Identifying outliers or anomalies in data by clustering normal data points together and flagging those that fall far from their cluster centroids, useful in fraud detection, network intrusion detection, and system monitoring.


## Constraints

To run the program, the following requirements should be met:

1. **Known number of data points**: The number of data points to be clustered should be known in advance.
2. **Data points in 2 dimensions**: The data points should be represented as (x, y) coordinates in a 2-dimensional space.
3. **Number of threads**: The number of threads used should be equal to the number of clusters specified when running the program.


