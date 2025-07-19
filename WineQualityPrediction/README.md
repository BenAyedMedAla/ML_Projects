# Wine Quality Prediction

This project aims to predict the quality of red wines based on various physicochemical properties using machine learning. The dataset contains different features related to the wine's chemical composition, and the goal is to classify wines into either "good" (quality >= 7) or "bad" (quality < 7) based on those features.

## Project Overview

In this project, we used a **Random Forest Classifier** to predict the quality of red wines. We first explored the dataset, visualized important relationships, and then pre-processed the data for training. The model was then evaluated using accuracy metrics.

The main steps of the project include:

1. **Data Exploration**: Understanding the features and relationships between them.
2. **Data Pre-processing**: Preparing the data for training by dropping unnecessary columns and performing label binarization.
3. **Model Training**: Training a Random Forest Classifier on the data.
4. **Model Evaluation**: Evaluating the model's performance using accuracy score.

## Dataset

The dataset is a collection of physicochemical properties of red wines. It contains the following columns:

- **Fixed acidity**
- **Volatile acidity**
- **Citric acid**
- **Residual sugar**
- **Chlorides**
- **Free sulfur dioxide**
- **Total sulfur dioxide**
- **Density**
- **pH**
- **Sulphates**
- **Alcohol**
- **Quality**: The target variable representing the quality of the wine (values range from 0 to 10).

### Target Variable:
- **Quality**: The quality of the wine, where:
  - 0 → Bad quality wine
  - 1 → Good quality wine (for this project, quality >= 7 is considered good)

## Key Features

The following features have shown strong relationships with wine quality:

- **Volatile acidity**: Inverse relationship with quality (higher volatile acidity typically leads to a lower quality wine).
- **Citric acid**: Direct relationship with quality (higher citric acid levels generally result in better quality wines).
- **Alcohol**: A key factor influencing the quality, with higher alcohol content often correlating with higher quality wines.
- **Sulphates**: Higher levels of sulphates may contribute to better quality wines.

## Steps Involved

### 1. Data Exploration

- **Dataset Inspection**: We first explored the dataset by loading it and checking for any missing values.
- **Visualizations**: We visualized the distribution of wine quality and the relationships between key features and wine quality using bar plots and a heatmap to identify correlations.

### 2. Data Pre-processing

- **Label Binarization**: The quality was binarized into two categories: wines with quality >= 7 (good) and wines with quality < 7 (bad).
- **Feature Selection**: We dropped the 'quality' column from the feature set to use it as the target variable.

### 3. Model Training

- **Model Selection**: We used a **Random Forest Classifier** to train the model on the pre-processed dataset.
- **Train-Test Split**: The dataset was split into training (80%) and test (20%) sets.

### 4. Model Evaluation

- **Prediction**: The model was used to predict the quality on the test data.
- **Accuracy**: The model's accuracy was evaluated using the `accuracy_score` metric, which measures the proportion of correctly classified instances.

## Results

The Random Forest Classifier achieved a high accuracy score in predicting the quality of wines based on the given features.

## Conclusion

This project demonstrates how machine learning can be applied to predict wine quality based on chemical features. The Random Forest model performed well, but future improvements can include tuning hyperparameters or using more advanced models.

## Requirements

- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn