# Music Genre Classification (PCA + MLP)

## Overview

This project classifies music genres using audio features from a large Spotify dataset. It combines data preprocessing, dimensionality reduction (PCA), and machine learning models to analyze and predict genres.

Project report: 

## Approach

* Cleaned dataset (50,000 songs) and removed non-numeric features
* Performed **train/test split before preprocessing** to avoid data leakage
* Encoded categorical features (key, mode)
* Applied **StandardScaler** for normalization
* Used **PCA (9 components, ~96.7% variance retained)** for dimensionality reduction
* Explored clustering structure (silhouette analysis)

## Models

* Random Forest
* XGBoost
* **MLP (best performing model)**

## Results

* **MLP Macro-AUC: ~0.924**
* Accuracy: ~56% (multi-class setting)
* Strong performance on distinct genres (e.g., Classical, Anime)
* Lower performance on overlapping genres (e.g., Hip-Hop, Alternative)
* PCA revealed only **2 well-separated clusters**, explaining classification difficulty 

## My Contributions

* Implemented **MLP model and evaluation pipeline**
* Designed **data preprocessing and PCA workflow**
* Conducted **model comparison and performance analysis**

## Technologies

* Python
* scikit-learn
* pandas, NumPy
* PCA, clustering, classification

## Notes

* Dataset contains overlapping feature distributions across genres
* PCA significantly improved model performance by reducing noise
* Focus on understanding feature space and model limitations
