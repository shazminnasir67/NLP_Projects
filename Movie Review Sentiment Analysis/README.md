# Movie Review Sentiment Analysis using Softmax Regression

This project focuses on sentiment analysis of movie reviews using Softmax Regression. The goal is to classify movie reviews into different sentiment categories based on the text data. The project includes data preprocessing, feature extraction (Bag of Words and N-Grams), and model training using Softmax Regression.

## Project Structure

The project is organized into the following files:

- **`data_preprocess.py`**: Reads the movie review dataset and prepares the data for feature extraction.
- **`feature_extraction.py`**: Implements feature extraction techniques such as Bag of Words and N-Grams.
- **`softmax_regerssion.py`**: Contains the implementation of the Softmax Regression model.
- **`main.py`**: The main script that ties everything together, including data loading, feature extraction, model training, and evaluation.

## Dataset

The dataset used in this project is the Kaggle Movie Review dataset, which contains phrases from movie reviews along with their sentiment labels. The dataset is stored in a TSV (Tab-Separated Values) format.

## Features

- **Bag of Words (BoW)**: Converts text data into a fixed-size vector by counting the frequency of each word in the text.
- **N-Grams**: Extracts sequences of N words (unigrams, bigrams, etc.) to capture more context in the text.

## Model

The **Softmax Regression** model is used for multi-class classification. It predicts the probability distribution over the sentiment classes and selects the class with the highest probability as the prediction.

## Usage

1. **Clone the repository**:
   ```bash
   git clone https://github.com/shazminnasir67/movie-review-sentiment-analysis.git
   cd movie-review-sentiment-analysis