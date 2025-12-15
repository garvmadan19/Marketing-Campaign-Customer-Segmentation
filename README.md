# Marketing-Campaign-Customer-Segmentation
Unsupervised machine learning project to cluster Rolling Stones songs based on Spotify audio features (K-Means &amp; PCA).

## Dataset
The primary dataset used for this project is a collection of Rolling Stones tracks from Spotify, which includes various audio features and popularity scores.

## Features and Methodology
The core of this project involves several key data science and machine learning techniques:
###  Data Cleaning & Preprocessing:
    - Handling of duplicate entries
    - Identification and removal of outliers in continuous variables such as `loudness`, `popularity`, and various audio features using the Interquartile Range (IQR) method
### Exploratory Data Analysis (EDA)
    - Analysis of album popularity to identify and recommend top-performing albums (e.g., "Sticky Fingers (Remastered)" and "Some Girls" were found to be the two most popular)
    - Visualization of song feature distributions (e.g., `acousticness`, `danceability`, `tempo`)
### Machine Learning:
    - Feature Scaling: Data features were scaled to ensure they contribute equally to the distance-based clustering algorithm.
    - Dimensionality Reduction: Principal Component Analysis (PCA) was used to reduce the number of features while retaining most of the variance in the data.
    - Clustering: The K-Means Clustering algorithm was applied to the reduced data to create song cohorts (clusters).
    - Evaluation: The optimal number of clusters was determined using techniques like the Elbow Method, and the clustering quality was evaluated using the Silhouette Score.

## Requirements
To run this project, you need a Python environment with the following libraries installed. You can install them using `pip`:
   - pip install pandas numpy matplotlib seaborn scikit-learn openpyxl

## Key Python Libraries Used:
 - pandas and numpy (For data manipulation) 
 - matplotlib.pyplot and seaborn (For data visualization) 
 - sklearn.preprocessing (For scaling/standardization) 
 - sklearn.decomposition.PCA (For dimensionality reduction) 
 - sklearn.cluster.KMeans (For the clustering algorithm) 
 - sklearn.metrics.silhouette_score (For cluster evaluation)

## 
