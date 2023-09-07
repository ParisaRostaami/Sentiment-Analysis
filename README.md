# Sentiment-Analysis
Sentiment Analysis using the "Sentiment Labelled Sentences" dataset from UCI, focusing on the Amazon dataset.

[![Contact](https://img.shields.io/badge/contact-Parisa.rostaamii%40gmail.com-yellow.svg)](mailto:Parisa.rostaamii@gmail.com)

# Sentiment Analysis on Amazon Cells Dataset

## Project Overview
This repository contains code for performing Sentiment Analysis using the "Sentiment Labelled Sentences" dataset from UCI. The primary focus is on analyzing the Amazon dataset. Sentiment Analysis is a type of classification that categorizes text data into positive or negative sentiments.

The project follows these main steps:
1. **Preprocessing**: The dataset is cleaned, including removing punctuation, converting text to lowercase, removing extra white spaces, and eliminating stopwords. Additionally, stemming and lemmatization are applied to the text data.
2. **Classification**: The preprocessed data is split into training and testing sets. Text data is transformed into numerical feature vectors using TF-IDF (Term Frequency-Inverse Document Frequency) vectorization. Two classification models, Multinomial Naive Bayes, and Logistic Regression, are trained on the TF-IDF transformed data and used for sentiment prediction.
3. **Evaluation & Comparison**: The models' performance is evaluated and compared using metrics such as confusion matrices, F1-Score, accuracy, and error rate.

## Preprocessing
- **Loading Packages**: Required libraries and packages are imported, including NLTK for natural language processing.
- **Loading and Preparing Dataset**: The Amazon dataset is loaded into a Pandas data frame, and columns are named as 'Sentence' and 'Class'. A temporary data frame ('temp') is created for storing preprocessed values.
- **Data Cleaning**: Punctuation is removed from sentences, letters are converted to lowercase, and extra white spaces are removed.
- **Stopword Removal**: NLTK's stopwords are removed from the sentences.
- **Stemming**: Words are stemmed using Porter Stemmer.
- **Lemmatization**: Words are lemmatized using WordNetLemmatizer.

## Classification
- **Data Splitting**: The preprocessed sentences and class labels are split into training and testing sets.
- **Text Vectorization (TF-IDF)**: TF-IDF vectorization is applied to convert text data into numerical feature vectors.

### Multinomial Naive Bayes
- A Multinomial Naive Bayes model is created and trained on the TF-IDF transformed training data.
- Predictions are made on the testing data.

### Logistic Regression
- A Logistic Regression model is created and trained on the TF-IDF transformed training data.
- Predictions are made on the testing data.

## Evaluation & Comparison
- For both Naive Bayes and Logistic Regression models, the following metrics are printed and compared:
   - Confusion matrix
   - F1-Score
   - Accuracy
   - Error rate

This code demonstrates the entire process of sentiment analysis, from data preprocessing to model evaluation and comparison using two different classification algorithms.

Feel free to explore the code and modify it for your own sentiment analysis tasks.
