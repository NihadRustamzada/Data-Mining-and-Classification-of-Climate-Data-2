# Project Overview
This project focuses on applying data mining techniques, including clustering and classification, to a climate dataset. The project explores hierarchical and K-Means clustering for discovering weather patterns and evaluates classifiers such as Random Forest, Support Vector Machine (SVM), and K-Nearest Neighbors (KNN) to classify data points based on the identified clusters.

The project is part of the M.Sc. Data Science curriculum at Lancaster University, under the SCC403: Data Mining course.

# Features
## Data Preprocessing
Cleaning, normalizing, standardizing, handling outliers, and feature transformation to prepare the data for further analysis.
## Dimensionality Reduction
Principal Component Analysis (PCA) to reduce the dataset’s dimensionality while retaining most of the variance.
## Clustering
K-Means and hierarchical clustering to group similar weather patterns.
## Classification
Random Forest, SVM, and KNN classifiers used to categorize new data points into the identified clusters.
## Cross-Validation
Evaluation of models using precision, recall, F1 score, and computational efficiency.
## Dataset
The dataset used for this project consists of 938 observations with five key meteorological features:

Temperature (°C)
Wind Speed (mph)
Wind Direction (degree)
Precipitation (mm)
Humidity (%)
# Data Preprocessing Steps
## Normalization and Standardization
Ensuring that each feature contributes equally to the analysis by normalizing the data.
## Outlier Detection
Using Interquartile Range (IQR) and Local Outlier Factor (LOF) methods to detect and remove outliers.
## Feature Transformation
Using trigonometric transformations for cyclical features like wind direction.
## Correlation Analysis
Removing highly correlated features to avoid redundancy.
## Principal Component Analysis (PCA)
Dimensionality reduction to retain key information while simplifying the dataset for clustering.
# Clustering Methods
## K-Means Clustering
Objective: Partition the dataset into K non-overlapping clusters.
Elbow Method: Used to determine the optimal number of clusters (K = 3 or K = 4).
Evaluation: Silhouette score and cluster centroids are analyzed for insight into different weather patterns.
## Hierarchical Clustering
Objective: Create a hierarchy of clusters using Ward’s method and Euclidean distance.
Dendrogram: Visualized the hierarchy and helped in determining four clusters.
Comparison with K-Means: Slightly better cluster definition based on evaluation metrics such as silhouette score.
# Classification Methods
Three classifiers were used to classify the clusters obtained from clustering techniques:

## Random Forest
Description: An ensemble learning technique that builds multiple decision trees.
Evaluation: F1 score of 90.4%, precision of 90.3%, and accuracy of 91.4%.
## Support Vector Machine (SVM)
Description: Constructs hyperplanes to separate different classes in high-dimensional space.
Evaluation: F1 score of 91.1%, precision of 91.1%, and accuracy of 92.2%.
## K-Nearest Neighbors (KNN)
Description: Classifies data based on the majority class of its nearest neighbors.
Evaluation: Best-performing classifier with an F1 score of 92.5%, precision of 92.5%, and accuracy of 93.3%.
# Results
K-Means Clustering: K = 3 provided the best-defined clusters based on silhouette scores.
Hierarchical Clustering: Achieved slightly better-defined clusters with a silhouette score of 0.417.
Classification: KNN outperformed SVM and Random Forest with higher accuracy and F1 scores, though SVM provided the best balance between accuracy and computational efficiency.
