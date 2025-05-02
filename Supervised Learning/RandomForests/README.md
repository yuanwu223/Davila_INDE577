# Random Forest Outlier Detection on Auction Verification Dataset

This repository demonstrates the application of the Random Forest algorithm for outlier detection using the `Auction Verification Regression with Anomalies` dataset. The notebook walks through the entire process, from data loading and preprocessing to model training and evaluation.

## Dataset Information

The dataset is sourced from [UCI Auction Verification Dataset](https://archive.ics.uci.edu/dataset/713/auction+verification) and contains anomaly scores of residual outliers obtained from a regression tree constructed on the auction verification data. The dataset consists of three columns:
- **RecordNum**: The sequence of records in the Auction Verification dataset.
- **Anomaly_Score**: The computed anomaly score for each record.
- **Outlier_Label**: The label indicating whether the record is an outlier or not ("Yes" or "No").

## Project Steps

### 1. Load and Explore the Dataset
- Import necessary libraries.
- Load the dataset into a DataFrame and inspect its structure, data types, and basic statistics.
- Check for missing values and handle them if necessary.

### 2. Data Preprocessing
- Encode categorical variables if any.
- Normalize or scale the features.
- Handle missing or anomalous data.
- Split the dataset into features (`X`) and target (`y`).

### 3. Train-Test Split
- Split the data into training and testing sets using an 80/20 split ratio.

### 4. Train Random Forest Model
- Initialize the Random Forest Regressor and fit the model to the training data.

### 5. Model Evaluation
- Evaluate the model performance using metrics such as Mean Absolute Error (MAE), Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and R² score.

### 6. Outlier Detection and Analysis
- Analyze the residuals by comparing predicted values with actual values.
- Evaluate how well the model identifies outliers using anomaly scores and labels.

### 7. Conclusion
- Summarize the model's performance and suggest potential improvements and further steps for better outlier detection.

## Requirements

This project requires the following Python libraries:
- `pandas`
- `numpy`
- `matplotlib`
- `scikit-learn`

To install the required dependencies, use the following command:
```bash
pip install -r requirements.txt
