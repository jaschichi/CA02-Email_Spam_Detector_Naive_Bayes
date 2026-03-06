# CA02-Email_Spam_Detector_Naive_Bayes
This project builds a Naive Bayes model to classify emails as spam or non-spam by cleaning email text, extracting the most frequent words, and evaluating the model’s prediction accuracy on a test dataset.

# Email Spam Detection using Naive Bayes

## Overview
This project builds a Naive Bayes classifier to detect whether an email is spam or not spam. The model is trained on labeled email data and then tested on unseen emails to evaluate its prediction accuracy. The workflow includes text preprocessing, feature extraction, model training, and evaluation.

## Dataset
The dataset contains two folders:

- train-mails: used to train the model  
- test-mails: used to evaluate the model  

The training dataset contains 702 labeled emails, equally divided between spam and non-spam. The model is evaluated using 260 test emails.

Email file naming patterns:

- number-numbermsg[number].txt → non-spam emails  
- spmsg[number].txt → spam emails  

## Methodology

### 1. Data Cleaning
Email text is cleaned by removing unnecessary words, symbols, and stop words that do not contribute to classification.

### 2. Feature Extraction
The program builds a dictionary using the 3000 most frequent words from the training dataset. Each email is then converted into a word frequency vector.

### 3. Model Training
A Naive Bayes classifier is trained using the processed training dataset.

### 4. Model Evaluation
The trained model predicts whether emails in the test dataset are spam or not spam, and the prediction accuracy is calculated.

## Technologies Used
- Python
- NumPy
- Pandas
- Scikit-learn
- Jupyter Notebook

## How to Run
1. Download or clone this repository.
2. Make sure the folders "train-mails" and "test-mails" are located in the same directory as the notebook.
3. Open the notebook in Jupyter Notebook or Google Colab.
4. Run all cells to train the model and evaluate the results.

## Purpose of the Assignment
The purpose of this assignment is to understand how text data is prepared for machine learning and how the Naive Bayes algorithm can be used for spam email classification.
