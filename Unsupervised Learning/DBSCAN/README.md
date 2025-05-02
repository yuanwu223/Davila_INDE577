# DBSCAN for Mall Customer Segmentation

## Overview

This project applies the **DBSCAN (Density-Based Spatial Clustering of Applications with Noise)** algorithm to perform customer segmentation on the **Mall Customer Segmentation** dataset. The goal is to identify customer segments based on **annual income** and **spending score** for targeted marketing strategies.

## Dataset

The dataset used in this project is the **Mall Customer Segmentation Data**, which includes the following features:

- **CustomerID**: Unique identifier for each customer.
- **Gender**: Gender of the customer.
- **Age**: Age of the customer.
- **Annual Income (k$)**: Annual income of the customer (in thousands of dollars).
- **Spending Score (1-100)**: A score assigned to customers based on their spending behavior.

## Steps

### 1. Data Loading
- Imported necessary libraries such as pandas, numpy, and scikit-learn.
- Loaded the dataset into a pandas DataFrame.

### 2. Exploratory Data Analysis (EDA)
- Checked for missing values and summarized basic statistics (mean, median, etc.).
- Visualized feature distributions and explored relationships between features.

### 3. Data Preprocessing
- Encoded categorical variables (e.g., `Gender`).
- Selected relevant features (e.g., **Annual Income** and **Spending Score**).
- Scaled the features using **StandardScaler**.

### 4. Apply DBSCAN
- Applied the **DBSCAN** algorithm from scikit-learn.
- Chose appropriate values for `eps` (maximum distance between two samples to be considered as in the same neighborhood) and `min_samples` (minimum number of points in a neighborhood for a point to be considered as a core point).
- Fit the DBSCAN model on the scaled features.

### 5. Analyze the Clustering Results
- Counted the number of clusters and noise points (points labeled as `-1`).
- Visualized the clusters using a scatter plot.
- Discussed the findings, such as which clusters correspond to high-income or high-spending customers, and identified outliers.

## Requirements

Make sure you have the following libraries installed:

- `pandas`
- `numpy`
- `scikit-learn`
- `matplotlib`
- `seaborn`

You can install them using pip:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn
