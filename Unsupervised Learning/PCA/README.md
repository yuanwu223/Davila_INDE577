# PCA on Online Retail Dataset

This project demonstrates the application of Principal Component Analysis (PCA) on the **Online Retail Dataset** to reduce the dimensionality and uncover underlying patterns in customer purchasing behavior. The dataset includes transactional data for a UK-based online retail store, which mainly sells unique all-occasion gifts.

## Project Overview

The goal of this project is to apply PCA to the Online Retail Dataset to reduce the dimensionality of the data and visualize customer purchasing patterns. Key steps in the project include:

1. **Data Preprocessing**: 
   - Loading and cleaning the dataset.
   - Filtering out canceled transactions and invalid entries.

2. **Feature Engineering**:
   - Aggregating data at the customer level (e.g., total quantity purchased, average unit price, total spending).
   - Standardizing the features to prepare them for PCA.

3. **Applying PCA**:
   - Using PCA to reduce the number of features while preserving as much variance as possible.
   - Determining the optimal number of components to retain.

4. **Visualizing PCA Results**:
   - Plotting the explained variance for each principal component.
   - Creating scatter plots to visualize clustering tendencies in the reduced feature space.

5. **Model Evaluation and Conclusion**:
   - Evaluate the effectiveness of PCA in reducing dimensionality while retaining the variance.
   - Summarize the insights gained from the PCA results and clustering analysis.

## Dataset

The **Online Retail Dataset** used in this project is available on Kaggle and contains the following key features:

- **InvoiceNo**: Unique identifier for each transaction.
- **StockCode**: Unique identifier for each product.
- **Quantity**: Number of items purchased in each transaction.
- **UnitPrice**: Price per unit of the product.
- **CustomerID**: Unique identifier for each customer.
- **InvoiceDate**: Date and time of the transaction.

The dataset spans all transactions from December 1, 2010, to December 9, 2011, for an online retail business primarily selling gifts.

## Steps

1. **Data Loading**: Load the Online Retail dataset and inspect its structure.
2. **Data Preprocessing**: Clean the dataset by handling missing values and removing invalid entries (e.g., canceled transactions and negative quantities).
3. **Feature Engineering**: Aggregate data at the customer level (e.g., total spent, total quantity purchased, etc.) and standardize the features.
4. **Applying PCA**: Apply PCA using `sklearn.decomposition.PCA` to reduce the dimensionality of the data while retaining as much variance as possible.
5. **Visualizing PCA Results**: Plot the explained variance and visualize the reduced data with scatter plots. Optionally, use clustering algorithms like KMeans to identify patterns.
6. **Model Evaluation and Conclusion**: Evaluate the results of the PCA transformation and the clustering analysis. Summarize the findings and discuss the insights gained from the data.

## Requirements

To run this project, you need to have the following libraries installed:

- `pandas`
- `numpy`
- `matplotlib`
- `scikit-learn`

You can install the necessary libraries by running:

```bash
pip install pandas numpy matplotlib scikit-learn
