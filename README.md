# CryptoClustering

This challenge, applies unsupervised learning to analyze cryptocurrency data and determine how 24-hour and 7-day price changes impact clustering results.

# Steps:
- Load crypto_market_data.csv into a DataFrame
- Standardize the data using StandardScaler
- Use the Elbow Method on the scaled dataset to determine the optimal number of clusters (k)
- Train a K-Means model with the best k and assign cluster labels
- Visualize clusters using a scatter plot (hvPlot)
- Apply Principal Component Analysis (PCA) to reduce the dataset to three principal components
- Compute explained variance to assess information retained
- Repeat the Elbow Method on the PCA-transformed data
- Compare the new optimal k with the original dataset
- Train K-Means on PCA data and visualize clusters
- Compare results from the original vs. PCA-reduced features
- Create composite plots to compare Elbow Curves and Cluster Visualizations
- Answer: How does using fewer features impact clustering?

#Analysis
- The PCA cluster optimization resulted in a 89.50% variance of the total variation in the original dataset
- Since 89.50% of the information was retained, the K-Means clustering of the PCA transformed data yields the same number of groupings that are more tightly grouped

  ![image](https://github.com/user-attachments/assets/e4dc71fa-5a23-4297-9446-67d2c8f8de45)
  
![image](https://github.com/user-attachments/assets/b0378719-4da0-44fc-86e2-31bbef2f639a)
