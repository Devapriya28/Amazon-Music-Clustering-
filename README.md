# Amazon-Music-Clustering

## 📌 Project Overview

With millions of songs on streaming platforms like Amazon Music, manually categorizing tracks into genres is impractical. This project uses unsupervised machine learning to automatically group similar songs based on their audio characteristics such as tempo, energy, danceability, and more.

By leveraging clustering techniques, we can uncover meaningful song groups that represent different genres, moods, or listening contexts — without any prior labels.

## 🚀 Skills You’ll Gain

Data Exploration & Cleaning

Feature Selection & Normalization

K-Means Clustering & Elbow Method

Cluster Evaluation (Silhouette Score, Davies-Bouldin Index)

Dimensionality Reduction (PCA, t-SNE)

Cluster Visualization & Interpretation

Python (pandas, NumPy, scikit-learn, matplotlib, seaborn)

Data Storytelling

## 🎯 Problem Statement

How can we automatically group songs with similar audio characteristics into clusters (potentially representing genres or moods), without relying on manual genre labels?

## 💡 Business Use Cases

Personalized Playlist Curation – Auto-generate playlists of similar-sounding tracks.

Improved Song Discovery – Suggest similar tracks based on user preferences.

Artist Analysis – Help artists identify competitors with similar sound profiles.

Market Segmentation – Enable streaming platforms to analyze listening trends.

## 🛠️ Approach
### 1. Data Exploration & Preprocessing

Load dataset: single_genre_artists.csv

Explore structure: columns, datatypes, nulls, duplicates

Drop unnecessary columns: track_id, track_name, artist_name

Normalize features using StandardScaler / MinMaxScaler

### 2. Feature Selection

Selected features for clustering:

danceability, energy, loudness, speechiness,

acousticness, instrumentalness, liveness, valence,

tempo, duration_ms

### 3. Dimensionality Reduction (Optional, for Visualization)

PCA (retain variance)

t-SNE (capture nonlinear relations)

### 4. Clustering Techniques

K-Means → Find k using Elbow Method & Silhouette Score

DBSCAN → Detect arbitrary-shaped clusters, noise/outliers

Hierarchical Clustering → Visualize merging via dendrogram

### 5. Cluster Evaluation

Silhouette Score – Cluster separation

Davies-Bouldin Index – Intra-cluster similarity

Inertia – Compactness of clusters

### 6. Visualization

2D scatter plots (PCA/t-SNE, color-coded clusters)

Bar charts → avg feature values per cluster

Heatmaps → feature comparisons

Distribution plots → tempo, danceability, etc.

### 7. Final Analysis

Add cluster labels to dataset

Profile clusters (e.g., high energy + danceability = Party tracks)

Export clustered dataset as CSV

Write a summary of cluster insights

## 📊 Results

By the end of the project, you will be able to:
✔️ Generate distinct clusters of songs based on audio features
✔️ Visualize clusters with PCA/t-SNE
✔️ Interpret each cluster (e.g., Party, Chill, Acoustic)
✔️ Support use cases like recommendation, playlisting, and trend analysis
