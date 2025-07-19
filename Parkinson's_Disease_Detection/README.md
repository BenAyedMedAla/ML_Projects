# Parkinson's Disease Detection

This project aims to detect Parkinson's Disease using machine learning techniques. We use **Support Vector Machine (SVM)** with a linear kernel to classify whether a person has Parkinson's Disease based on various medical features.

## Project Overview

Parkinson's Disease is a progressive neurological disorder that affects movement. The goal of this project is to develop a model that can predict whether an individual has Parkinson's Disease based on features extracted from medical tests. The dataset used in this project contains various features that reflect voice characteristics of individuals, which are key in detecting Parkinson’s Disease.

The steps involved in this project are:

1. **Data Collection & Analysis**: Loading the dataset, inspecting its structure, and performing exploratory data analysis (EDA).
2. **Data Pre-processing**: Separating the features and target, splitting the data into training and testing sets, and standardizing the features.
3. **Model Training**: Using Support Vector Machine (SVM) with a linear kernel to train the model.
4. **Model Evaluation**: Evaluating the model’s performance using accuracy scores on both training and test data.
5. **Predictive System**: Building a predictive system that takes user input and classifies whether the individual has Parkinson's Disease or not.

## Dataset

The dataset used for this project contains various voice features and the target variable `status`, which indicates whether the individual has Parkinson's Disease or not.

- **Features**: Various voice features such as jitter, shimmer, and other acoustic measures that are useful in identifying Parkinson's Disease.
- **Target Variable** (`status`): 
  - 1 → Parkinson's Positive
  - 0 → Healthy

## Steps Involved

### 1. Data Collection & Analysis

- The dataset is loaded into a Pandas DataFrame and inspected for missing values and statistical measures.
- The distribution of the target variable `status` (Parkinson's Positive or Healthy) is analyzed.

### 2. Data Pre-processing

- **Separation of Features and Target**: The features (X) are separated from the target variable (`status`).
- **Splitting the Data**: The data is split into training and test datasets using an 80-20 split.
- **Data Standardization**: The data is standardized using `StandardScaler` to ensure that all features are on the same scale, which helps improve model performance.

### 3. Model Training

- **Support Vector Machine (SVM)**: A linear kernel SVM is used for classification.
- The model is trained using the training data and then used to make predictions on both the training and test data.

### 4. Model Evaluation

- **Accuracy Score**: The model’s performance is evaluated using accuracy scores, which are calculated on both the training and test datasets.

### 5. Predictive System

- The trained model can predict whether a person has Parkinson’s Disease or not based on input data. For instance, input data includes various voice features, which are transformed and standardized before being passed to the model for prediction.

## Key Features

The dataset includes the following important features that are used for prediction:

- **Jitter**: A measure of frequency variation in the voice.
- **Shimmer**: A measure of amplitude variation in the voice.
- **Noise-to-Harmonic Ratio**: A measure of vocal quality.
- **Other Acoustic Features**: Various voice-related features that capture different characteristics of speech patterns.

## Model

- **Support Vector Machine (SVM)**: We use SVM with a linear kernel for classification. SVM is known for its ability to work well with high-dimensional data, making it suitable for this project.
- **Standardization**: We standardize the input data using `StandardScaler` to ensure better model performance, especially when features have different scales.

## Conclusion

This model is capable of classifying individuals as either having Parkinson's Disease or not based on acoustic features of their speech. The model’s accuracy can be further improved by experimenting with different algorithms, feature engineering, or more advanced pre-processing techniques.

## Requirements

- Python 3.x
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn