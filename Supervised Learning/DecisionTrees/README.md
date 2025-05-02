# Decision Trees for Student Performance Estimation

## Overview

This project implements a Decision Tree algorithm to predict student performance based on various features like study hours, absences, and school support. The dataset used simulates student performance data, and the goal is to predict the final grade of students.

## Dataset

The dataset used in this project is the **Student Performance Estimation Dataset**, which includes the following features:
- **student_id**: Unique ID for each student (S0001–S1000)
- **study_hours**: Total study time per week
- **absences**: Number of absences
- **school_support**: Whether the student received school-provided academic support
- **final_grade**: Final exam score (0–100)

## Steps

### 1. Data Loading
- Imported necessary libraries such as pandas, numpy, and scikit-learn.
- Loaded the dataset into a DataFrame.

### 2. Exploratory Data Analysis (EDA)
- Checked for missing values and summarized basic statistics (mean, median, etc.).
- Visualized feature distributions and explored relationships between features.

### 3. Data Preprocessing
- Encoded categorical variables (e.g., `school_support`).
- Split the dataset into training and testing sets.

### 4. Model Building
- Initialized a Decision Tree Classifier and trained it on the training dataset.

### 5. Model Evaluation
- Evaluated model performance using metrics such as accuracy, precision, recall, F1-score, and the confusion matrix.
- Visualized feature importance to understand the most influential factors in predicting student performance.

### 6. Hyperparameter Tuning 
- Optimized hyperparameters such as `max_depth`, `min_samples_split`, and `criterion` using Grid Search.

### 7. Model Interpretation
- **Decision Tree Visualization**: Visualized the trained decision tree to interpret how the model makes predictions based on different features.
- **Feature Importance**: Analyzed the importance of each feature in predicting the final grade, identifying the most significant features.

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
