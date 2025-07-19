# Medical Insurance Cost Prediction

This project aims to predict the medical insurance costs for individuals based on various factors like age, gender, BMI, number of children, smoking status, and region. We use a **Linear Regression** model to predict the insurance cost.

## Project Overview

In this project, we built a predictive model using **Linear Regression** to estimate the medical insurance costs based on personal and demographic information. The dataset consists of both categorical and numerical features, and we performed the necessary data pre-processing to encode the categorical variables before training the model.

The main steps of the project are:

1. **Data Collection & Analysis**: Loading the dataset and performing exploratory data analysis (EDA).
2. **Data Pre-processing**: Encoding categorical features and splitting the data into features and target.
3. **Model Training**: Training a Linear Regression model using the training dataset.
4. **Model Evaluation**: Evaluating the model using R-squared scores for both training and test datasets.
5. **Building a Predictive System**: Developing a simple interface to make predictions based on user input.

## Dataset

The dataset contains the following features:

- **age**: The age of the individual.
- **sex**: The gender of the individual (male or female).
- **bmi**: Body Mass Index (BMI) of the individual.
- **children**: The number of children/dependents covered by the insurance.
- **smoker**: Whether the individual smokes (yes or no).
- **region**: The region in which the individual resides (southeast, southwest, northeast, northwest).
- **charges**: The medical insurance charges for the individual (target variable).

### Categorical Features:
- Sex
- Smoker
- Region

### Target Variable:
- Charges (insurance cost)

### Requirements

-Python 3.x

-pandas

-numpy

-matplotlib

-seaborn

-scikit-learn