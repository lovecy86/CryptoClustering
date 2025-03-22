# Cryptocurrency Clustering using K-Means and PCA

## Project Overview
This project analyzes cryptocurrency market data by applying K-Means clustering and Principal Component Analysis (PCA) to group similar cryptocurrencies based on their price change percentages over different time periods.

## Key Steps
### Data Preprocessing:
Loaded cryptocurrency market data.
Standardized numerical features using StandardScaler to normalize the dataset.

### Finding the Optimal Number of Clusters (k):
Used the Elbow Method to determine the best k value by plotting inertia vs. cluster count.
The optimal value of k was found to be 4 for both the original and PCA-transformed data.
[Elbow Curve][Images/elbow_curve.png]

### Clustering and Visualization:
Applied K-Means clustering on both the original scaled data and the PCA-reduced data.
Generated scatter plots to visualize cluster distributions.
[Scatter Plot][Images/scatter_plot.png]

### Impact of PCA on Clustering:
PCA reduced dimensionality while retaining ~89% of the variance in just 3 principal components.
Clustering on PCA-reduced data resulted in more compact clusters, and boundaries between groups became less distinct.

## Conclusion
Using PCA for clustering reduces complexity while maintaining meaningful patterns. However, it can also make clusters appear more compressed, potentially affecting the interpretability of results.

