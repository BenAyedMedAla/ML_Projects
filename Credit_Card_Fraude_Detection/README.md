# Credit Card Fraud Detection

This project aims to detect fraudulent credit card transactions using machine learning. The dataset contains both normal and fraudulent transactions, with the goal of training a model to accurately predict whether a given transaction is legitimate or fraudulent.

## Project Overview

In this project, we used a **Logistic Regression** model to classify transactions as either legitimate or fraudulent. The dataset used for this project is highly imbalanced, with fewer fraudulent transactions compared to normal transactions. The main steps of the project include:

1. **Data Preprocessing**: Handling missing values, understanding data distribution, and balancing the dataset.
2. **Model Training**: Training a Logistic Regression model on the balanced dataset.
3. **Model Evaluation**: Evaluating the model's performance on both the training and test datasets using accuracy score.

## Dataset

The dataset used in this project is the **Credit Card Fraud Detection Dataset**, which contains transaction data with the following columns:

- **Time**: The number of seconds elapsed between this transaction and the first transaction in the dataset.
- **V1, V2, V3, ..., V28**: The 28 anonymized features generated using PCA (Principal Component Analysis) to protect the confidentiality of the original dataset.
- **Amount**: The amount of the transaction.
- **Class**: The target variable, where:
  - 0 → Legitimate Transaction
  - 1 → Fraudulent Transaction

### Dataset Imbalance

The dataset is highly imbalanced, with a very small percentage of fraudulent transactions compared to legitimate ones.

### Requirements

-Python 3.x

-pandas

-numpy

-scikit-learn