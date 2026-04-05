# \# Customer Segmentation with K-Means, DBSCAN, and PCA

# 

# This project applies unsupervised machine learning techniques to segment customers based on purchasing behavior and demographic data. The goal is to identify meaningful customer groups that can be used to drive targeted marketing strategies and improve business decision-making.

# 

# \---

# 

# \## Problem Overview

# 

# Customer segmentation is a key component of marketing analytics. By grouping customers with similar behaviors and characteristics, businesses can tailor campaigns, optimize product placement, and improve customer engagement.

# 

# This project uses clustering algorithms to uncover natural groupings within customer data, with a focus on interpretability and actionable insights.

# 

# \---

# 

# \## Dataset

# 

# \- Source: Kaggle (Customer Personality Analysis Dataset)

# \- Records: \~2,200 customers

# \- Features: Demographics, purchasing behavior, and campaign responses

# 

# The dataset includes variables such as income, spending across product categories, purchase frequency, and marketing campaign engagement.

# 

# Note: The dataset is not included in this repository due to file size.

# 

# \---

# 

# \## Approach

# 

# The full workflow is implemented in a single notebook and includes:

# 

# \### 1. Data Preparation

# 

# \- Data cleaning and removal of missing values

# \- Feature engineering (e.g., customer age, total spending)

# \- One-hot encoding of categorical variables

# \- Feature scaling using StandardScaler

# 

# \### 2. Exploratory Data Analysis

# 

# \- Distribution analysis of key variables

# \- Correlation analysis to understand feature relationships

# \- Initial insights into customer behavior patterns

# 

# \### 3. Model Development

# 

# Two clustering algorithms were applied and compared:

# 

# \- K-Means Clustering

# \- DBSCAN

# 

# Model selection was based on:

# 

# \- Silhouette score

# \- Visual inspection using PCA-reduced data

# 

# \### 4. Dimensionality Reduction

# 

# \- Principal Component Analysis (PCA) was applied to:

# &#x20; - Reduce dimensionality

# &#x20; - Improve clustering performance

# &#x20; - Enable visualization of clusters

# 

# \### 5. Evaluation

# 

# \- Elbow method (inertia)

# \- Silhouette score

# \- Cluster visualization using PCA

# 

# \---

# 

# \## Results

# 

# \- Optimal clustering achieved with \*\*K-Means (k = 2)\*\*

# \- PCA improved clustering performance:

# &#x20; - Silhouette score increased from \~0.197 to \~0.213

# 

# \### Key Insights

# 

# \- One cluster represents \*\*high-income, high-spending customers\*\*

# \- The other cluster represents \*\*lower-spending customers\*\*

# \- Spending variables (e.g., wine, meat, premium products) were the strongest differentiators

# \- Demographic variables had less influence compared to behavioral features

# 

# \---

# 

# \## Repository Structure

# 

# ```text

# Customer-Segmentation/

# │

# ├── data/

# │   └── README.md

# ├── notebooks/

# │   └── customer\_segmentation\_kmeans\_dbscan\_pca.ipynb

# ├── src/

# │   └── utils.py

# ├── requirements.txt

# └── .gitignore

