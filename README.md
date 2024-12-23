# Files Overview
**1. analysis.py** :
This script performs data preprocessing, sentiment analysis model training, and evaluation. Key steps include:

Loading and cleaning the dataset using pandas and nltk.
Preprocessing text data with tokenization, stopword removal, and lemmatization.
Converting text to TF-IDF vectors with TfidfVectorizer.
Training a LogisticRegression model to classify sentiments.
Evaluating model performance using metrics like accuracy, confusion matrix, and classification report.
Saving the trained model and vectorizer as .pkl files for deployment.


**2. app.py** :
This is a Flask web application for serving the sentiment analysis model. Key features include:

A homepage (/) that displays an interface for user input.
An endpoint (/predict) for predicting sentiment from user-provided reviews.
Integration with the predict_sentiment function (presumably from the model module) for real-time predictions.
Handles exceptions and provides clear error messages in the API responses.

**3. vectorizer.pkl** :
A serialized object containing the trained TF-IDF vectorizer used to transform text data into feature vectors. This is loaded by the application or model for consistent feature extraction during inference.
