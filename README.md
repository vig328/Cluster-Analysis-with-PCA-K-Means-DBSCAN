- Intoduction

This Jupyter Notebook explores unsupervised learning techniques using K-Means, DBSCAN, and PCA. The goal is to generate synthetic datasets, apply clustering methods, and visualize how they perform, especially after dimensionality reduction.

-  What’s Inside the Notebook?

The notebook starts by importing essential Python libraries:
  
  1- numpy, pandas → data handling

  2-matplotlib, seaborn → data visualization

  3-scikit-learn (KMeans, DBSCAN, PCA, make_blobs, make_moons) → clustering & dimensionality reduction

  4-standardScaler → feature scaling

-  Generating Synthetic Data

-  Two types of datasets are created for experiments:

- Blobs Dataset (make_blobs)

Creates well-separated spherical clusters.

Useful for testing how well algorithms detect distinct groups.

- Moons Dataset (make_moons)

Creates two crescent-shaped clusters.

Useful for testing algorithms on non-linear cluster shapes.

Example visualization:

plt.scatter(X_blobs[:,0], X_blobs[:,1], c=y_blobs) shows 4 blob clusters.

-  K-Means Clustering

  K-Means is applied on the blobs dataset.

Process:

fit → Learns 4 cluster centers from the data.

predict → Assigns each data point to the nearest cluster.

Output:

A label (0,1,2,3) for each point.

Centroids marked as red “X”.

Visualization clearly shows circular cluster boundaries, which work well for blobs.

- DBSCAN (Density-Based Spatial Clustering)

PCA is used for dimensionality reduction.

It reduces high-dimensional data into 2D or 3D for visualization.

Preserves as much variance as possible while reducing complexity.

Helps visualize clustering results more clearly.

- Comparison & Insights

K-Means is great for spherical blobs but struggles with non-linear data.

DBSCAN adapts better to irregular shapes and identifies noise.

PCA makes visualization possible in 2D while retaining key features.

- Applications of This Project

Customer segmentation in marketing

Detecting fraud or anomalies

Grouping similar patterns in data

Reducing data complexity for visualization

