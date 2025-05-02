# XGBoost Regression on NYC Airbnb Open Data

This repository demonstrates the application of the XGBoost algorithm for predicting Airbnb listing prices using the `New York City Airbnb Open Data` dataset. The notebook walks through the entire process, including data loading, preprocessing, model training, hyperparameter tuning, and evaluation.

## Dataset Information

The dataset is sourced from [Inside Airbnb](http://insideairbnb.com/get-the-data/), and includes listing-level data from New York City. Key columns include:
- **latitude / longitude**: Geolocation of the property.
- **room_type**: Type of Airbnb room (Entire home, Private room, etc.).
- **minimum_nights**: Minimum stay duration.
- **number_of_reviews**: Total number of reviews.
- **availability_365**: Availability of the listing throughout the year.
- **price**: Target variable representing the listing price.

## Project Steps

### 1. Load and Explore the Dataset
- Import necessary libraries.
- Load the dataset into a DataFrame.
- Inspect structure, data types, and summary statistics.
- Handle missing values or drop irrelevant features.

### 2. Data Preprocessing
- Encode categorical variables (e.g., `room_type`).
- Normalize or scale numeric features if necessary.
- Filter out unreasonable price or nights entries.
- Split the dataset into features (`X`) and target (`y`).

### 3. Train-Test Split
- Split the data into training and testing sets using an 80/20 ratio.

### 4. Train XGBoost Model
- Initialize the XGBoost Regressor.
- Train the model on the training data.

### 5. Hyperparameter Tuning
- Use GridSearchCV to search for the best combination of hyperparameters:
  - `learning_rate`
  - `max_depth`
  - `n_estimators`
  - `subsample`
  - `colsample_bytree`

### 6. Model Evaluation
- Evaluate model performance on the test set using:
  - Mean Absolute Error (MAE)
  - Mean Squared Error (MSE)
  - Root Mean Squared Error (RMSE)
  - R² Score

### 7. Feature Importance and Interpretation
- Extract and visualize feature importance.
- Interpret which features have the most impact on price prediction.

### 8. Conclusion
- Summarize the model’s performance and tuning results.
- Discuss potential improvements such as using other ML models or integrating more features.

## Requirements

This project requires the following Python libraries:

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `xgboost`

Install dependencies with:
```bash
pip install -r requirements.txt
