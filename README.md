# Unsupervised Learning - Clustering Analysis on Fashion-MNIST Dataset
Project Overview
This project, part of a machine learning course at the University of Macedonia, involves applying unsupervised learning techniques to the Fashion-MNIST dataset. The goal is to determine the most efficient clustering algorithm and the optimal number of clusters by evaluating multiple performance metrics. Clustering is performed on both the raw data and data transformed using Principal Component Analysis (PCA).

Dataset
The Fashion-MNIST dataset is used in this project, containing images of fashion products classified into 10 categories. However, the project focuses on clustering the data into fewer clusters (3-12) to evaluate clustering quality using various metrics.

Key Objectives
Apply clustering algorithms to both raw data and PCA-transformed data.
Identify the best clustering algorithm and number of clusters by evaluating clustering performance scores.
Compare clustering performance on raw vs PCA-transformed data.
## Methods
Data Preprocessing
Train-Test Split: The dataset was split into training (54,000 samples), testing (6,000 samples), and validation (10,000 samples) sets.
PCA: Principal Component Analysis (PCA) was applied to reduce the dimensionality of the dataset, retaining 95% of the original variance.
Clustering Techniques
Three clustering algorithms were applied to both raw and PCA-transformed data:

K-Means Clustering
Mini-Batch K-Means Clustering
Gaussian Mixture Model
Clustering was performed for various cluster sizes (3-12) to determine the optimal number of clusters.

Performance Metrics
The clustering performance was evaluated using the following metrics:

Silhouette Score: Measures how similar a point is to its cluster compared to other clusters.
Calinski-Harabasz Index: A higher score indicates better-defined clusters.
Davies-Bouldin Index: A lower score indicates better clustering.
Fowlkes-Mallows Index: Measures the similarity between two clusters, where a higher score indicates a better match.

## Results
Best Clustering Results
Raw Data:
K-Means performed best, especially with 4 clusters, achieving strong clustering performance.
PCA-Transformed Data:
Gaussian Mixture Model yielded better results compared to K-Means and Mini-Batch K-Means, especially when clustering into 7 clusters.
Optimal Number of Clusters:
For raw data, 4 clusters provided the best results across all metrics.
For PCA-transformed data, the best results were obtained with 7 clusters.

## Visualizations
Several visualizations, such as Silhouette Scores, Calinski-Harabasz Scores, and Davies-Bouldin Scores, were generated to compare clustering performance across different algorithms and cluster sizes.

## Conclusion and Future Improvements
The K-Means algorithm worked best for raw data, while Gaussian Mixture performed better on PCA-transformed data.
To improve clustering accuracy, testing additional clustering methods, such as hierarchical clustering, and adjusting PCA parameters could provide better results.
Clustering on 10 clusters (matching the actual categories of Fashion-MNIST) should be explored for practical purposes, despite the best results being observed with fewer clusters.
## Contributors
Charalambia Zerva (ics20117)
Maria-Anna Ioannidou (ics20067)
Alexandros Lemona (ics20103)
