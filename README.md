# CryptoClustering
module 19

# Overview
In this challenge, you'll use your knowledge of Python and unsupervised learning to predict if cryptocurrencies are affected by 24-hour or 7-day price changes.

# Instructions
- Load and scale the crypto market data.
- Use the Elbow Method to determine the optimal number of clusters (`k`).
- Apply K-Means clustering using both the scaled data and PCA-reduced data.
- Visualize the clusters with interactive `hvPlot` scatter plots.
- Compare cluster results between the full dataset and the PCA-reduced dataset.

# Questions and Answers:

**Question:** What is the best value for `k`?

**Answer:** The best value for k is 4 because inertia sharply decreases.


**Question:** What is the total explained variance of the three principal components?

**Answer:** The total explained variance of the three principal components is about 0.895, meaning that about 89.5% of the original dataset's information is retained after dimensionality reduction using PCA. 


**Question:** What is the best value for `k` when using the PCA data?

**Answer:** The best value for k when using the PCA data is 4 because the Elbow curve flattens noticeably after this point. 

**Question:** Does it differ from the best k value found using the original data?

**Answer:** No, the best value for k is the same for both the original scaled data and the PCA-reduced data. This suggests that reducing the features to three principal components preserved the key structure of the dataset.
 

**Question:** After visually analyzing the cluster analysis results, what is the impact of using fewer features to cluster the data using K-Means?

**Answer:** Using fewe3r features through PCA simplifies the dataset while preserving most of its variability. After visually analyzing the cluster analysis results, the clusters from the PCA-reduced data are generally similar in structure to those from the full dataset but may appear more compact or slightly shifted. This suggests that PCA effectively reduces dimensionality without significantly sacrificing clustering quality, making the analysis more efficient and visually interpretable. However, some fine details or subtle distinctions between clusters may be lost due to the reduction in features.
