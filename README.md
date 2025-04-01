# Spam-sms-detection

Dataset Handling

The dataset spam.csv is uploaded in Google Colab.

It contains two essential columns:

v1: Label (Spam/Ham)

v2: Email message text

Extra columns are removed for cleaner processing.

Text Preprocessing

Converts text to lowercase.

Removes special characters.

Tokenizes text and removes stopwords (common words like "the," "is").

Feature Extraction (TF-IDF Vectorization)

Converts processed text into numerical format using TF-IDF (Term Frequency-Inverse Document Frequency).

Helps the model understand important words in the dataset.

Model Training (Naïve Bayes Classifier)

Splits the dataset into 80% training and 20% testing.

Uses Multinomial Naïve Bayes, which is effective for text classification tasks.

Model Evaluation

Predicts spam or ham on the test dataset.

Prints:

Accuracy

Classification Report (Precision, Recall, F1-score)

Saving & Downloading the Model

The trained model (spam_detector.pkl) and vectorizer (vectorizer.pkl) are saved and downloaded.

These files can be used later for spam detection without retraining the model.

Spam Prediction Function

A function (predict_email) takes any email text input.

It preprocesses, vectorizes, and predicts if the email is spam or ham.

