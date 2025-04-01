# Sms_Spam_Detection

# Overview
This project implements a Spam Detection System using machine learning to classify text messages as either Spam (unwanted messages) or Ham (legitimate messages). The system uses a Multinomial Naive Bayes classifier trained on a dataset of labeled SMS messages.

# Features
Text Preprocessing: Uses TF-IDF vectorization to convert text into numerical features.

Model Training: Multinomial Naive Bayes classifier for efficient spam detection.

Evaluation Metrics: Reports accuracy, precision, and confidence scores.

Interactive Demo: Allows users to input messages and get real-time predictions.

# Dataset
Source: spam.csv (SMS Spam Collection Dataset)

Columns:

target: Label (ham or spam)

text: SMS message content

Size: 5,169 messages after cleaning (removing duplicates).

# Performance Metrics
Accuracy: 97.29%

Precision: 100% (No false positives in spam detection)

Confidence Scores: Provided for each prediction.

# How It Works
Data Cleaning:

Drops unnecessary columns.

Encodes labels (ham=0, spam=1).

Removes duplicate messages.

Text Vectorization:

Uses TfidfVectorizer to convert messages into TF-IDF features (limited to 3,000 most frequent words).

Model Training:

Splits data into 80% training and 20% testing sets.

Trains a MultinomialNB classifier.

Prediction:

Users can input messages to get instant spam/ham classification with confidence scores.

# Usage
Running the Code
Ensure dependencies are installed:

Use jupyter notebook or google colab 

pip install numpy pandas scikit-learn
Place spam.csv in the same directory as the notebook.

Run the Jupyter notebook (Spam_Detection.ipynb).

# Dependencies
Python 3.8+

Libraries:

pandas

numpy

scikit-learn

# License
MIT License. Free for academic and commercial use.
