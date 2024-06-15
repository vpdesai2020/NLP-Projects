# Restaurant Review Classification

This repository contains a Natural Language Processing (NLP) project focused on classifying restaurant reviews into positive and negative sentiments. The project involves preprocessing text data, creating a Bag-of-Words model, and implementing a Multinomial Naive Bayes classifier for sentiment analysis.

## Project Structure

- **Imports and Downloads:**  
  - Imports necessary libraries such as `nltk` for text processing and `sklearn` for machine learning tasks. Downloads stopwords and tokenizer if not already present.

- **Data Cleaning:**  
  - Defines a function to clean text data by removing non-alphabetic characters, converting text to lowercase, tokenizing, removing stopwords, and applying stemming using NLTK's Porter Stemmer.

- **Bag-of-Words Model:**  
  - Utilizes `CountVectorizer` from `sklearn.feature_extraction.text` to transform cleaned text data into a numerical matrix (Bag-of-Words model) where each row represents a document and columns represent word frequencies.

- **Naive Bayes Classification:**  
  - Splits the dataset into training and testing sets, trains a Multinomial Naive Bayes classifier on the training data, and evaluates its performance on the test data.

- **Evaluation Metrics:**  
  - Calculates accuracy, generates a classification report (precision, recall, F1-score), and constructs a confusion matrix to assess model performance in predicting sentiment (positive or negative) from restaurant reviews.

## Results

The Multinomial Naive Bayes model achieved an accuracy of 74.5% on predicting sentiment from unseen restaurant reviews. It demonstrated balanced precision and recall scores for both positive and negative sentiment classes, as indicated by the classification report and confusion matrix.

## Conclusion

This project illustrates a structured approach to sentiment analysis using NLP techniques and supervised learning. The choice of Multinomial Naive Bayes was appropriate given the nature of the data and the features derived from the Bag-of-Words model.
