# K-Nearest Neighbors (KNN) on Forest Cover Type Dataset

This Jupyter notebook demonstrates how to apply the K-Nearest Neighbors (KNN) algorithm to classify the Forest Cover Type dataset. The dataset consists of cartographic variables for forested areas, aiming to predict the type of forest cover.

## Dataset

- **Dataset Name**: Forest Cover Type Dataset
- **Description**: This dataset contains tree observations from four areas of the Roosevelt National Forest in Colorado. It includes various cartographic variables such as elevation, aspect, slope, distance to hydrology, soil type, and more.
- **Target Variable**: Forest cover type (7 different classes)
- **Data Source**: UCI Machine Learning Repository / Kaggle

### Features:
- **Elevation**
- **Aspect**
- **Slope**
- **Distance to Hydrology**
- **Soil Type**
- **Hillshade**
- **Other Cartographic Variables**

### Target:
- **Forest Cover Type** (7 different classes)

## Steps in the Notebook

### Step 1: Data Loading
The dataset is loaded and checked for missing values and any inconsistencies.

### Step 2: Data Preprocessing
- **Feature Selection**: We remove the target variable from the feature set.
- **Train-Test Split**: The dataset is split into training and testing sets (80% training, 20% testing).
- **Feature Scaling**: Standardization is applied to scale the features, ensuring that all features contribute equally to the distance calculations in KNN.

### Step 3: Model Training
The K-Nearest Neighbors (KNN) classifier is initialized and trained on the training data. The `k` value is initially set to 5.

### Step 4: Model Evaluation
After training the model, predictions are made on the test data, and the performance is evaluated using:
- **Accuracy Score**
- **Classification Report** (Precision, Recall, F1-score for each class)
- **Confusion Matrix** (Visualized using a heatmap)

## Requirements

- Python 3.x
- Libraries:
  - `numpy`
  - `pandas`
  - `matplotlib`
  - `seaborn`
  - `scikit-learn`

## How to Run the Notebook

1. Clone this repository to your local machine.
2. Install the required libraries:
   ```bash
   pip install -r requirements.txt
