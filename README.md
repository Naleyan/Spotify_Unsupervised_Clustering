# 🎵 Spotify Unsupervised Learning Challenge 🎵

Academic project carried out as part of the Fundamentals of Machine Learning (FML)** module – IMT Atlantique (FISE A2, 2025).  
The goal of this project is to **explore and analyze musical trends on Spotify (2010–2022)** using **unsupervised learning techniques** such as PCA, K-Means, and t-SNE.

## 📁 Project Structure

"""
Spotify-Unsupervised_Learning_Challenge/
│
├── data/
│ ├── raw/ # Raw data (original Spotify CSV)
│ └── processed/ # Cleaned and preprocessed data for modeling
│
├── notebooks/ # Jupyter notebooks for each project stage
│ ├── 01_EDA.ipynb # Exploratory Data Analysis
│ ├── 02_Preprocessing.ipynb
│ ├── 03_Clustering.ipynb
│ └── 04_Analysis.ipynb
│
├── src/ # Modular Python scripts
│ ├── data_preprocessing.py
│ ├── feature_engineering.py
│ ├── clustering_models.py
│ └── init.py
│
├── requirements.txt # Python dependencies
└── README.md # This file
"""


## 🧠 Project Objectives

1. **Analyze** the audio characteristics of 2,300 popular tracks (2010–2022).  
2. **Clean, normalize, and transform** the data to make it suitable for unsupervised models.  
3. **Apply PCA and K-Means** to identify latent structures among Spotify tracks.  
4. **Interpret** the resulting clusters and their musical meaning.  


## ⚙️ Data Processing Pipeline

1. **Exploration (EDA)**
- Statistical analysis of 23 variables  
- Detection of outliers and missing values  
- Study of distributions (normality, skewness, correlations)  

2. **Preprocessing**
- Removal of missing or inconsistent entries  
- Separation between metadata and numerical features  
- Semantic grouping of genres (`genre_grouped2`)  
- Standardization using `StandardScaler`  

3. **Dimensionality Reduction**
- Application of **Principal Component Analysis (PCA)**  
- Axis interpretation:  
  - **PC1** → energy / valence  
  - **PC2** → danceability / production  

4. **Clustering**
- Models: **K-Means**, **GMM**, **t-SNE**  
- Metrics: Inertia, Silhouette Score, Davies-Bouldin, Calinski-Harabasz  
- 2D visualizations using PCA and t-SNE projections  

5. **Analysis & Interpretation**
- Identification of 5 main musical archetypes:
  - **Dance/Pop** (high energy, modern tracks)
  - **Spoken Word** (high speechiness)
  - **Acoustic** (low energy, high acousticness)
- Observation of a **continuous sound spectrum**, rather than distinct genre clusters.  


## 📊 Key Results

- Dataset: 2,300 tracks, 23 audio features  
- PCA: first two components explain ≈ 50% of variance  
- Optimal K-Means: **k = 6**  
- Silhouette Score ≈ 0.07 → low cluster separation  
- Main insight: **music forms a continuous spectrum of characteristics** rather than distinct, separable groups.  



## 🚀 Future Work

If the unsupervised constraint were lifted:
- **Popularity Prediction** (regression task)
- **Automatic Genre Classification** (supervised learning – Random Forest, SVM)
- Possible extension to a **music recommendation system**



## 🧰 Technical Environment

Installation: pip install -r requirements.txt


## 👨‍💻 Project Team

Achraf ESSALEH; 
Sara ELBARI;
Eva LANSALOT;
Houda DAOUAIRI;
Kalis KRAÏFI;
Nada ALEIAN;




Supervised by IMT Atlantique – FISE A2 (2025)
Module: Fundamentals of Machine Learning (DASCI)
