# Yelp Review Sentiment Analysis with Neural Networks

This project implements a neural network model to analyze Yelp reviews and predict the sentiment (positive or negative) based on user ratings. The dataset used for this analysis is the [Yelp Reviews Dataset](https://www.yelp.com/dataset), which contains business reviews, ratings, and other related data.

## Project Overview

The goal of this project is to build a neural network model that can classify Yelp reviews into positive or negative sentiment categories based on the review text. The project involves several key steps:

1. **Data Preprocessing**: 
   - Loading and cleaning the dataset.
   - Converting the review text into a format suitable for input into a neural network model.
   
2. **Text Cleaning**: 
   - Removing special characters and converting text to lowercase to standardize the input.
   
3. **Tokenization**:
   - Using Keras' `Tokenizer` to convert the review text into sequences of integers.
   
4. **Padding**:
   - Padding the sequences to ensure that all inputs are of equal length.

5. **Model Training**:
   - Using a neural network model to train the dataset on a classification task.

## Dataset

The project uses the Yelp Academic Dataset, which includes the following files:

- `yelp_academic_dataset_review.json`: Contains reviews including review text, ratings, and user information.
- `yelp_academic_dataset_business.json`: Contains business information such as name, location, and categories.
- `yelp_academic_dataset_checkin.json`: Contains check-in information indicating how often users have checked into a business.

For this project, the focus is on the `yelp_academic_dataset_review.json` file, which contains the review text and ratings.

## Steps

1. **Data Loading**: Load a subset of the Yelp review dataset.
2. **Data Preprocessing**: Clean the text and prepare it for tokenization.
3. **Tokenization**: Convert the text into sequences of integers using Keras' `Tokenizer`.
4. **Padding**: Pad the tokenized sequences to ensure consistent input lengths.
5. **Model Training**: Train the neural network model on the preprocessed data.
6. **Evaluation**: Evaluate the model's performance on a test set.

## Requirements

To run this project, you need to have the following libraries installed:

- `pandas`
- `numpy`
- `tensorflow`
- `sklearn`

You can install the necessary libraries by running:

```bash
pip install -r requirements.txt
