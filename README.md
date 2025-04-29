
Spam Detection
This project implements a spam detection system using machine learning. The system classifies text messages as either "spam" or "ham" (non-spam) based on the contents of the message.

Project Overview
The system is built using Python and uses the Naive Bayes classifier combined with TF-IDF (Term Frequency-Inverse Document Frequency) for feature extraction. The steps involved are as follows:

Data Preprocessing:
The data is cleaned by removing unwanted columns.
Labels are mapped to the categories spam and ham.
The text is preprocessed by converting to lowercase, removing numbers, and stripping punctuation.

Data Balancing
The dataset is balanced by ensuring an equal number of "spam" and "ham" messages for training.

Model Building:
A machine learning pipeline is built using a TF-IDF vectorizer and Multinomial Naive Bayes classifier.

Model Evaluation:
The model is evaluated using a classification report that includes metrics such as precision, recall, and F1-score.

Model Saving:
The trained model and vectorizer are saved for future use.

Requirements
Python 3.x
Libraries:numpy,pandas,re,sklearn,pickle

Usage
1. Preprocessing and Training
The script automatically reads a dataset (CSV file) and preprocesses it for model training. You can adjust the dataset by providing a different path to the data = pd.read_csv(...) function.

2. Model Evaluation
After training the model, the classification report will be printed, showing the performance metrics.

3. Saving the Model
Once the model is trained, both the trained model and vectorizer are saved as .pkl files:
spam_classifier.pkl: Contains the Naive Bayes classifier and TF-IDF vectorizer pipeline.
vectorizer.pkl: Contains the saved vectorizer, useful for transforming new input text data.
