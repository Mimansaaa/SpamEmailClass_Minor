# Spam Email Classification Project

## Overview

This Java-based project focuses on classifying emails into two categories: spam and ham (non-spam). The classification is performed using three different algorithms: Naive Bayes, Logistic Regression, and Decision Tree. The project utilizes the Term Frequency-Inverse Document Frequency (TF-IDF) technique to calculate the importance of each word in the emails, enabling effective analysis and classification.

## Features

- **Naive Bayes Algorithm:** This algorithm is employed for its simplicity and efficiency in text classification tasks. It assumes independence between features and is well-suited for analyzing the presence of words in spam and ham emails.

- **Logistic Regression:** Logistic regression is used as a probabilistic model to predict the probability of an email being spam or ham. It's particularly useful for binary classification problems.

- **Decision Tree Algorithm:** Decision trees provide a structured way to make decisions based on features. In this project, a decision tree is employed to identify key features in the emails that contribute to their classification as spam or ham.

- **TF-IDF Calculation:** The TF-IDF technique is used to evaluate the significance of each word in the emails. It considers both the frequency of a term within a document (TF) and its rarity across all documents (IDF). This helps in capturing the importance of words in distinguishing between spam and ham.

## Project Structure

The project is organized into the following components:

1. **Data Preprocessing:** The raw email data is preprocessed to extract relevant features and convert them into a format suitable for machine learning algorithms. This includes tokenization, stemming, and TF-IDF calculation.

2. **Algorithm Implementation:** Each of the three algorithms (Naive Bayes, Logistic Regression, and Decision Tree) is implemented for email classification.

3. **Evaluation:** The performance of each algorithm is assessed using various metrics, including confusion matrices. The confusion matrix provides a detailed breakdown of the model's predictions, showing true positives, true negatives, false positives, and false negatives.

    ### Confusion Matrix

    A confusion matrix is a table that summarizes the performance of a classification algorithm. Here is how the confusion matrix is interpreted in the context of spam email classification:

    |               | Predicted Spam | Predicted Ham   |
    |---------------|----------------|------------------|
    | Actual Spam   | True Positive  | False Negative  |
    | Actual Ham    | False Positive | True Negative   |

    - **True Positive (TP):** The number of spam emails correctly classified as spam.
    - **True Negative (TN):** The number of ham emails correctly classified as ham.
    - **False Positive (FP):** The number of ham emails incorrectly classified as spam.
    - **False Negative (FN):** The number of spam emails incorrectly classified as ham.

    ### Performance Metrics

    In addition to confusion matrices, the following metrics are used to evaluate the performance of each algorithm:

    - **Accuracy:** The proportion of correctly classified emails.
    - **Precision:** The ability of the classifier not to label as spam emails that are not spam.
    - **Recall (Sensitivity):** The ability of the classifier to find all the spam emails.
    - **F1 Score:** The harmonic mean of precision and recall, providing a balanced measure.

4. **User Interface (Optional):** A user interface may be included to facilitate user interaction, allowing users to input new emails for classification.

