## Social Media Post Clustering and Analysis

# Overview

This project involves clustering social media posts based on various metrics such as the number of reactions, comments, shares, and different types of reactions (likes, loves, wows, etc.). The analysis uses K-Means and Hierarchical Clustering to identify patterns and group similar posts.

# Dataset

The dataset contains social media posts with the following columns:

- `status_id`: Unique identifier for each post.
- `status_type`: Type of post (e.g., video, photo).
- `status_published`: Date and time the post was published.
- `num_reactions`: Total number of reactions.
- `num_comments`: Total number of comments.
- `num_shares`: Total number of shares.
- `num_likes`: Total number of likes.
- `num_loves`: Total number of loves.
- `num_wows`: Total number of wows.
- `num_hahas`: Total number of hahas.
- `num_sads`: Total number of sads.
- `num_angrys`: Total number of angrys.
- `Column1`, `Column2`, `Column3`, `Column4`: Additional columns (currently not used in analysis).

The dataset file is `Live.csv`.

## Objectives

1. **Cluster social media posts** using K-Means and Hierarchical Clustering methods.
2. **Evaluate clustering performance** using the Silhouette Score.
3. **Visualize the clusters** to understand the distribution of posts across clusters.

## Data Preprocessing

1. **Load the Dataset**: The data is read from `Live.csv`.
2. **Feature Selection**: Columns from index 3 to 12 are selected for clustering.
3. **Standardization**: Features are standardized using `StandardScaler`.

## Clustering

1. **K-Means Clustering**:
   - Determine the optimal number of clusters using the Elbow Method.
   - Apply K-Means clustering with the determined number of clusters.
   - Calculate the Silhouette Score to evaluate clustering quality.

2. **Hierarchical Clustering**:
   - Generate a dendrogram to visualize the hierarchical clustering structure.

## Visualization

- **Clusters Visualization**: Scatter plots are used to visualize clusters based on the first two features.
- **Dendrogram**: Visualize the hierarchical clustering of data.

## Results

- **Elbow Method**: Determines the optimal number of clusters by plotting the WCSS (Within-Cluster Sum of Squares).
- **Silhouette Score**: Provides a measure of how well the clusters are separated and cohesive and the score is 0.7499921477392748.
- **Cluster Visualization**: Displays clusters and centroids on a scatter plot.
- **Dendrogram**: Shows the hierarchical clustering structure of the dataset.
