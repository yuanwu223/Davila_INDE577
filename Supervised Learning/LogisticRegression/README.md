# Logistic Regression on Social Network Ads Dataset

This Jupyter Notebook applies the Logistic Regression algorithm to predict whether a user will purchase a product based on their age, gender, and estimated salary. The dataset used is the **Synthetic Logistic Regression Dataset** from Kaggle, which is specifically designed for practicing logistic regression techniques.

## Table of Contents

1. [Introduction](#introduction)
2. [Dataset Description](#dataset-description)
3. [Steps to Apply Logistic Regression](#steps-to-apply-logistic-regression)
   - [Data Loading and Exploration](#1-data-loading-and-exploration)
   - [Data Preprocessing](#2-data-preprocessing)
   - [Model Building](#3-model-building)
   - [Model Evaluation](#4-model-evaluation)
   - [Results Interpretation](#5-results-interpretation)
4. [Results](#results)

## Introduction

This project demonstrates the application of the Logistic Regression algorithm to classify users based on their likelihood of purchasing a product. The dataset contains several user features, including age, gender, and estimated salary, and the target variable indicates whether the user made a purchase.

## Dataset Description

The dataset used in this project is the **Synthetic Logistic Regression Dataset**. It includes the following columns:

- **User ID**: Unique identifier for each user
- **Gender**: Gender of the user (Male/Female)
- **Age**: Age of the user
- **EstimatedSalary**: Estimated annual salary of the user
- **Purchased**: Target variable (0 = No, 1 = Yes)

### Data Format

The data is in CSV format, and the following is a snippet of the dataset:

| User ID  | Gender | Age | EstimatedSalary | Purchased |
|----------|--------|-----|-----------------|-----------|
| 15624510 | Male   | 19  | 19000           | 0         |
| 15810944 | Male   | 35  | 20000           | 0         |
| 15668575 | Female | 26  | 43000           | 0         |
| ...      | ...    | ... | ...             | ...       |

## Steps to Apply Logistic Regression

### 1. Data Loading and Exploration
- Load the dataset and inspect its structure.
- Check for missing values and handle them if necessary.
- Display the first few rows of the dataset.

### 2. Data Preprocessing
- Convert categorical columns (such as **Gender**) into numerical values using encoding.
- Standardize the features (Age and EstimatedSalary) if necessary.
- Split the data into features (X) and target (y).
- Split the dataset into training and test sets (80% training, 20% test).

### 3. Model Building
- Import and instantiate the Logistic Regression model.
- Train the model using the training data.

### 4. Model Evaluation
- Evaluate the model using metrics such as accuracy, precision, recall, F1 score, and confusion matrix.
- Visualize the results using a confusion matrix and ROC curve.

### 5. Hyperparameter Tuning (Optional)
- Use techniques like GridSearchCV to optimize hyperparameters and re-train the model.

### 6. Results Interpretation
- Analyze the model's coefficients and understand the importance of different features.
- Discuss how the model's predictions can be applied in a business context.

## Results

The model achieved the following evaluation metrics:

- **Accuracy**: 88.75%
- **Precision**: 91.30%
- **Recall**: 75.00%
- **F1 Score**: 82.35%

The results suggest that the model performs well with a balance between precision and recall.

## Conclusion

The Logistic Regression model demonstrates good performance in predicting whether a user will purchase a product based on the given features. While the precision is high, improving recall could be beneficial for targeting more true positive cases (purchases). This analysis can help businesses identify and target customers who are more likely to make a purchase based on their demographic data.

## Requirements

To run this Jupyter Notebook, the following Python libraries are required:

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

## Installation

Install the necessary libraries using pip:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
