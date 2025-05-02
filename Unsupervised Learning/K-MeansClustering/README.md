# K-Means Clustering on Credit Card Dataset

This repository demonstrates the application of the K-Means Clustering algorithm for customer segmentation using the `Credit Card Dataset`. The notebook walks through the entire process, from data loading and preprocessing to clustering, analyzing, and interpreting the results.

## Dataset Information

The dataset is sourced from [UCI Credit Card Dataset](https://archive.ics.uci.edu/ml/datasets/default+of+credit+card+clients) and contains information about credit card customers' spending behavior and demographic features. The dataset includes the following columns:
- **BALANCE**: The balance on the credit card.
- **BALANCE_FREQUENCY**: The frequency of the balance.
- **PURCHASES**: The total amount of purchases made.
- **ONEOFF_PURCHASES**: The amount spent in one-off purchases.
- **INSTALLMENTS_PURCHASES**: The amount spent in installments.
- **CASH_ADVANCE**: The cash advance amount.
- **PURCHASES_FREQUENCY**: The frequency of purchases.
- **ONEOFF_PURCHASES_FREQUENCY**: The frequency of one-off purchases.
- **PURCHASES_INSTALLMENTS_FREQUENCY**: The frequency of installment purchases.
- **CASH_ADVANCE_FREQUENCY**: The frequency of cash advances.
- **CASH_ADVANCE_TRX**: The number of cash advance transactions.
- **PURCHASES_TRX**: The number of purchase transactions.
- **CREDIT_LIMIT**: The credit limit of the customer.
- **PAYMENTS**: The total amount paid by the customer.
- **MINIMUM_PAYMENTS**: The minimum amount due on the account.
- **PRC_FULL_PAYMENT**: The percentage of full payments made.
- **TENURE**: The number of months the customer has had the credit card.

## Project Steps

### 1. Load and Explore the Dataset
- Import necessary libraries.
- Load the dataset into a DataFrame and inspect its structure, data types, and basic statistics.
- Check for missing values and handle them if necessary.

### 2. Data Preprocessing
- Handle missing values by filling or imputing the data.
- Remove or transform irrelevant features (e.g., `CUST_ID`).
- Scale the numerical features to standardize the data.
- Handle any outliers that could affect clustering.

### 3. Feature Selection
- Select the relevant features for clustering, excluding irrelevant ones.
- Optionally, apply dimensionality reduction techniques (e.g., PCA) to reduce the number of features.

### 4. Determine the Optimal Number of Clusters
- Use the **Elbow Method** to determine the optimal number of clusters by plotting the Within-Cluster Sum of Squares (WCSS) for different values of k.
- Optionally, validate the number of clusters using the **Silhouette Score**.

### 5. Apply K-Means Clustering
- Initialize the K-Means model with the optimal number of clusters (k).
- Fit the K-Means model to the scaled data and assign each data point to a cluster.

### 6. Analyze the Clusters
- Inspect the cluster centroids to understand the characteristics of each cluster.
- Analyze the distribution of data points across clusters.
- Identify key patterns or trends in each cluster (e.g., high spenders, low credit limit users).

### 7. Interpret the Results and Define Marketing Strategy
- Based on the clustering results, define actionable marketing strategies for each customer segment (e.g., tailored promotions for high spenders, adjusting credit limits for low-credit customers).
- Discuss the business implications of the customer segments and suggest strategies for targeted marketing.

### 8. Conclusion
- Summarize the findings from the customer segmentation analysis.
- Discuss the impact of these insights on marketing strategies and potential areas for improvement.

## Requirements

This project requires the following Python libraries:
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`

To install the required dependencies, use the following command:
```bash
pip install -r requirements.txt