# SMS Spam Collection using Naïve Bayes

## Overview

This project implements a **spam filter for SMS and email messages** using the **Naïve Bayes machine learning algorithm**. The system processes text messages, extracts relevant textual features, and classifies each message as either **spam** or **ham (legitimate)**.

The project follows a practical machine learning workflow, from text preprocessing and feature extraction to model training, evaluation, model export, and prediction on unseen messages.

## Objectives

* Understand the Naïve Bayes algorithm for text classification.
* Preprocess SMS and email text for machine learning.
* Apply tokenization and stop-word removal.
* Convert text into numerical features.
* Train a Naïve Bayes spam classifier.
* Evaluate the classifier using unseen test data and performance metrics.
* Identify suspicious keywords and patterns associated with spam.
* Export the trained model for later use.
* Build a spam-filtering tool capable of classifying text from an input file.

## Problem Statement

Spam messages are a common cybersecurity and communication-security problem. A large volume of unwanted messages can contain advertisements, phishing attempts, malicious links, scams, or other potentially harmful content.

The goal of this project is to develop a machine learning-based spam filter that can automatically distinguish between:

* **Spam** — unwanted or potentially suspicious messages.
* **Ham** — legitimate messages.

The classifier learns textual patterns from a labeled dataset rather than relying on a manually defined list of suspicious keywords.

## Machine Learning Workflow

```text
SMS / Email Dataset
        ↓
Text Data Loading
        ↓
Text Preprocessing
        ↓
Tokenization & Stop-word Removal
        ↓
Feature Extraction
        ↓
Train / Test Split
        ↓
Naïve Bayes Classifier
        ↓
Model Evaluation
        ↓
Export Trained Model
        ↓
New SMS / Email
        ↓
Spam or Ham Prediction
```

## Text Preprocessing

The text data is prepared before training the classifier. The preprocessing pipeline may include:

* Converting text to a consistent case
* Tokenization
* Removing unnecessary characters
* Removing stop words
* Cleaning whitespace
* Preparing text for feature extraction

These steps reduce unnecessary variation in the input data and help the classifier focus on meaningful textual patterns.

## Feature Extraction

Machine learning algorithms require numerical input, so the processed messages are transformed into numerical feature vectors.

The project uses text feature extraction to represent messages based on their words and word frequencies. These representations allow the Naïve Bayes classifier to learn which textual patterns are more strongly associated with spam or legitimate messages.

## Naïve Bayes Classifier

The core model is a **Naïve Bayes classifier**, a probabilistic algorithm that is particularly effective for many text-classification problems.

The classifier estimates the probability that a message belongs to each class based on the words and features present in the message.

For spam filtering, the model learns relationships such as:

```text
Message Features
       ↓
Probability of Spam
       +
Probability of Ham
       ↓
Predicted Class
```

The "naïve" assumption is that features are conditionally independent given the class. Despite this simplifying assumption, Naïve Bayes often performs very well on high-dimensional text data.

## Model Evaluation

The trained classifier is evaluated using previously unseen messages.

Important evaluation metrics include:

* Accuracy
* Precision
* Recall
* F1-score
* Confusion Matrix

These metrics help determine how effectively the spam filter detects unwanted messages while avoiding incorrect classification of legitimate messages.

## Dynamic Spam Detection

Rather than manually specifying suspicious words, the model **learns important textual patterns from the training dataset**.

For example, words and phrases frequently occurring in spam messages can contribute to a higher probability of a message being classified as spam.

This makes the system more adaptable than a rule-based filter based only on manually defined keywords.

## Model Export and Prediction

After training and evaluation, the trained spam classifier can be exported and reused without retraining.

The prediction workflow is:

```text
Input Text File
      ↓
Read Message
      ↓
Apply Same Preprocessing
      ↓
Transform Using Saved Features
      ↓
Load Trained Naïve Bayes Model
      ↓
Predict
      ↓
SPAM / HAM
```

This demonstrates how a machine learning model can move from experimentation to a reusable spam-filtering application.

## Cybersecurity Applications

The techniques demonstrated in this project can be applied to:

* SMS spam detection
* Email spam filtering
* Phishing message detection
* Malicious-message classification
* Social engineering detection
* Security message screening
* Automated communication filtering
* Text-based threat detection

## Technologies

* **Python 3.x**
* **Scikit-learn**
* **Pandas**
* **NLTK**
* **Jupyter Notebook**

## Key Concepts

* Naïve Bayes
* Bayes Theorem
* Text Classification
* Spam Detection
* Natural Language Processing
* Tokenization
* Stop-word Removal
* Feature Extraction
* TF-IDF / Text Vectorization
* Supervised Learning
* Model Evaluation
* Precision
* Recall
* F1-score
* Confusion Matrix
* Model Serialization
* Cybersecurity Analytics

## Project Structure

```text
SMS-Spam-Collection-Naive-Bayes/
│
├── SMS_Spam_Collection_Naive_Bayes.ipynb
└── README.md
```

## Learning Outcome

This project provides practical experience in applying **machine learning and natural language processing to a cybersecurity problem**. It demonstrates how a Naïve Bayes classifier can learn from labeled SMS/email data and be transformed into a reusable spam-filtering system.

The project also establishes a foundation for more advanced cybersecurity applications involving **NLP, phishing detection, malicious-content classification, and automated threat detection**.

## Course Information

**Course:** AI for Cybersecurity
**Lab:** SMS Spam Collection using the Naïve Bayes Spam Filter
**Algorithm:** Naïve Bayes
**Domain:** Cybersecurity / Natural Language Processing
**Language:** Python
