# The Perceptron Algorithm - Machine Learning Model

This repository contains the implementation of the **Perceptron** algorithm from scratch. The Perceptron is a simple yet effective linear classifier that is widely used in binary classification tasks.

## Overview

The notebook `ThePerceptron.ipynb` demonstrates the following:

1. **Preprocessing the Dataset**: 
   - Loading and preparing the dataset.
   - Handling missing data and encoding categorical variables.
   
2. **Implementing the Perceptron Model**:
   - A custom implementation of the Perceptron algorithm.
   - Training the model with the dataset and making predictions.

3. **Model Evaluation**:
   - Accuracy calculation for the Perceptron model.
   - Visualization of the data and model predictions using a scatter plot.

## Steps

### 1. Data Preprocessing

- The dataset is loaded and preprocessed, including:
  - Dropping the target column for features (`X`).
  - Handling any missing values using mean imputation.
  - Splitting the data into training and testing sets (80% training, 20% testing).
  
### 2. Perceptron Algorithm

The Perceptron algorithm is implemented manually in the following steps:

- **Step 1**: Initialize weights and bias.
- **Step 2**: Iterate over the training data and update weights based on prediction errors.
- **Step 3**: Repeat until convergence or a maximum number of iterations.

### 3. Model Training and Evaluation

- The model is trained using the training set and tested on the test set.
- The accuracy of the model is calculated by comparing predicted labels with the actual labels in the test set.
  
### 4. Visualizing the Results

- A scatter plot of two features (`age` and `trestbps`) is generated to visualize the training data and predictions.
- The plot uses color coding to show the predicted labels (0 or 1) for each data point.

## Results

The Perceptron algorithm achieves an **accuracy of 81.95%** on the test data, indicating a relatively good performance on this dataset.

## Dependencies

To run this notebook, you need the following Python libraries:

- `numpy`
- `pandas`
- `matplotlib`
- `sklearn`

You can install the required libraries using `pip`:

```bash
pip install numpy pandas matplotlib scikit-learn
