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

# \- Optimal clustering achieved with K-Means (k = 2)

# \- PCA improved clustering performance:

# &#x20; - Silhouette score increased from \~0.197 to \~0.213

# 

# \### Key Insights

# 

# \- One cluster represents high-income, high-spending customers

# \- The other cluster represents lower-spending customers

# \- Spending variables were the strongest differentiators

# \- Demographic variables had less influence compared to behavioral features

# 

# \---

# 

# \## Repository Structure

# 

# &#x20;   Customer-Segmentation/

# &#x20;   ├── data/

# &#x20;   │   └── README.md

# &#x20;   ├── notebooks/

# &#x20;   │   └── customer\_segmentation\_kmeans\_dbscan\_pca.ipynb

# &#x20;   ├── src/

# &#x20;   │   └── utils.py

# &#x20;   ├── requirements.txt

# &#x20;   └── .gitignore

# 

# \---

# 

# \## How to Run

# 

# 1\. Clone the repository:

# &#x20;  git clone https://github.com/Jorge-Barajas-Github/Customer\_Segmentation\_Using\_Unsupervised\_Learning.git

# 

# 2\. Install dependencies:

# &#x20;  pip install -r requirements.txt

# 

# 3\. Download the dataset (see data/README.md) and place it in:

# &#x20;  data/raw/

# 

# 4\. Run the notebook:

# &#x20;  jupyter notebook

# 

# \---

# 

# \## Limitations

# 

# \- Clustering results depend on feature selection and scaling

# \- DBSCAN performance is sensitive to parameter tuning

# \- Only two clusters identified, which may oversimplify customer behavior

# \- Limited temporal analysis of customer activity

# 

# \---

# 

# \## Future Improvements

# 

# \- Explore additional clustering methods (e.g., hierarchical clustering)

# \- Tune DBSCAN parameters more extensively

# \- Incorporate time-based features for longitudinal analysis

# \- Use clustering outputs for downstream supervised models

# 

# \---

# 

# \## References

# 

# Fernandes, S. (2022). Customer Personality Analysis \[Data set]. Kaggle.  

# https://www.kaggle.com/datasets/imakash3011/customer-personality-analysis

# 

# Scikit-learn developers. (2024). Scikit-learn: Machine Learning in Python.  

# https://scikit-learn.org/stable/index.html

# 

# \---

