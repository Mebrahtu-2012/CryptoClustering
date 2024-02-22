# Cryptocurrency Clustering Analysis

## Overview
This repository contains code for performing clustering analysis on cryptocurrency market data using the K-Means algorithm. The analysis involves clustering cryptocurrencies based on their price change percentages over 24 hours and 7 days. Two approaches are explored: one using the original scaled data and the other using Principal Component Analysis (PCA)-transformed data.

## Steps

1. **Data Loading and Exploration:**
   - Load the cryptocurrency market data from the provided CSV file.
   - Display summary statistics and visualize the data to understand its structure.

2. **Data Preparation:**
   - Normalize the data using StandardScaler from scikit-learn.
   - Create a DataFrame with the scaled data and set the 'coin_id' index.

3. **Cluster Analysis with Original Scaled Data:**
   - Utilize the elbow method to determine the optimal number of clusters (k).
   - Initialize and fit a K-Means model with the best value of k.
   - Predict clusters and add a new column to the DataFrame with cluster labels.
   - Visualize the clusters using a scatter plot.

4. **PCA for Dimensionality Reduction:**
   - Conduct Principal Component Analysis (PCA) to reduce the dimensionality of the data.
   - Assess the total explained variance of the principal components.
   - Create a DataFrame with the PCA-transformed data.

5. **Cluster Analysis with PCA Data:**
   - Apply the elbow method to identify the optimal number of clusters using PCA-transformed data.
   - Initialize and fit a K-Means model with the best value of k obtained from PCA.
   - Predict clusters and add a new column to the PCA DataFrame with cluster labels.
   - Visualize the clusters using a scatter plot.

6. **Analysis and Interpretation:**
   - Evaluate the impact of using fewer features for clustering with K-Means.
   - Discuss the differences between clustering results obtained from original scaled data and PCA-transformed data.

## Requirements
- Implement the elbow method to find the best value for k using both original and PCA-transformed data.
- Initialize and fit K-Means models with the best k values obtained from both approaches.
- Visualize clusters using scatter plots and assess the clustering performance.
- Answer provided questions related to the analysis.

## References
- [hvplot documentation](https://hvplot.holoviz.org/getting_started/hvplot.html)
- Classroom activities and materials provided during the course

