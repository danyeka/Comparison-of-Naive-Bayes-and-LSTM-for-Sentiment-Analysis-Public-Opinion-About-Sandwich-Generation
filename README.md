## Comparison of Naive Bayes and LSTM for Sentiment Analysis Public Opinion About Sandwich Generation

**This repository contains the implementation of a sentiment analysis project comparing the performance of the Naive Bayes and Long Short-Term Memory (LSTM) algorithms in analyzing public opinion about the Sandwich Generation on Twitter.**

# Table of Contents

- Introduction
- Dataset
- Preprocessing
- Algorithms
- Naive Bayes
- LSTM
- Evaluation
- Results and Comparison
- Usage
- Acknowledgments

# Introduction

The Sandwich Generation refers to individuals supporting both their aging parents and children simultaneously. This phenomenon is often discussed on social media platforms like Twitter. This study compares Naive Bayes and LSTM algorithms to analyze public sentiment (positive, negative, neutral) about this issue.

Key findings:
- **LSTM** achieved higher accuracy (**91.85%**) than **Naive Bayes** (**83%**).
- **LSTM** excelled in handling complex and long-text data.

# Dataset

Source: Tweets collected via Twitter API using the keyword "sandwich generation."
Period: January 1, 2019 – October 13, 2024.
Size: 3,769 tweets (increased to 6,193 after augmentation).

# Preprocessing

Steps to prepare data for analysis:

- Case Folding: Convert text to lowercase.
- Cleaning: Remove punctuation, special characters, and URLs.
- Tokenization: Split text into individual words (tokens).
- Normalization: Correct informal words to standard forms.
- Stopword Removal: Eliminate non-informative words (e.g., "and", "the").
- Stemming: Reduce words to their root forms.

# Algorithms

**Naive Bayes**

**Type**: Multinomial Naive Bayes.
**Strengths**: Fast and simple for text classification.
**Limitations**: Struggles with complex sentence structures and dependencies.

**LSTM**

**Type**: Recurrent Neural Network variant designed for sequence data.
**Strengths**: Captures long-term dependencies in text.

**Hyperparameters**:
- **Best Batch Size**: 64
- **Best Epochs**: 150
- **Optimal Neurons**: 75

# Evaluation
Metrics used for model performance:

- **Accuracy**
- **Precision**
- **Recall**
- **F1-Score**

Evaluation was performed using the SMOTE technique for class balancing and confusion matrix for detailed performance analysis.


# Results and Comparison

| Algorithm     | Accuracy (%)  | Precision (%) | Recall (%) | F1=Score |
| --------------| --------------| ------------- | -----------|----------|
| Naive Bayes   | 83            | 90            | 82         | 86       |
| LSTM          | 91.79         | 91.79         | 91.85      | 91.76    |


# Acknowledgments

**Special thanks to Helmi Satria and Twitter API for providing the dataset and Anas Fajri as friends in helping resolve errors.**