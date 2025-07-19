# Titanic Survival Prediction using Machine Learning

This project aims to predict whether a passenger on the Titanic survived or not based on a set of features such as age, gender, class, and other details. The model used in this project is **Logistic Regression**.

## Project Overview

The Titanic Survival Prediction project involves using a machine learning model to classify passengers as either survived or not. The model is trained on historical data from the Titanic disaster, where the goal is to predict survival based on passenger characteristics.

The main steps of the project are:

1. **Data Collection & Processing**: Loading and exploring the dataset.
2. **Handling Missing Values**: Pre-processing the data by handling missing values.
3. **Data Analysis & Visualization**: Analyzing the dataset and visualizing the distribution of features.
4. **Encoding Categorical Features**: Converting categorical variables into numerical representations.
5. **Model Training & Evaluation**: Training the model using logistic regression and evaluating its performance.
6. **Model Performance**: Evaluating the model's accuracy using training and test data.

## Dataset

The Titanic dataset contains the following key features:

- **PassengerId**: A unique identifier for each passenger.
- **Pclass**: The class of the passenger (1st, 2nd, or 3rd).
- **Sex**: The gender of the passenger.
- **Age**: The age of the passenger.
- **SibSp**: The number of siblings or spouses aboard the Titanic.
- **Parch**: The number of parents or children aboard the Titanic.
- **Fare**: The fare paid by the passenger.
- **Embarked**: The port where the passenger boarded the Titanic (C = Cherbourg; Q = Queenstown; S = Southampton).
- **Survived**: The target variable (1 = survived, 0 = did not survive).

### Key Features

- **Survived**: This is the target variable we are predicting.
- **Sex**: Gender plays an important role in predicting survival.
- **Age**: Age of the passenger can influence survival probability.
- **Pclass**: Class of the ticket is an important factor in determining survival.
- **Embarked**: Port of embarkation is relevant to the passengers' survival chances.

### Data Preprocessing

- **Missing Values**: Missing data in the `Age` and `Embarked` columns are handled. For the `Age` column, missing values are replaced with the mean age, and for the `Embarked` column, missing values are replaced with the mode.
- **Dropping Columns**: The `Cabin` column is dropped due to a high percentage of missing values.
- **Encoding Categorical Data**: The categorical features `Sex` and `Embarked` are encoded into numerical values to make them suitable for the machine learning model.

## Data Analysis & Visualization

The following visualizations were used to explore and understand the data:

- **Survival Distribution**: A count plot of survival (0 for did not survive, 1 for survived).
- **Gender Distribution**: A count plot of the `Sex` column to show how gender affects survival.
- **Pclass Distribution**: A count plot showing the relationship between ticket class and survival.
- **Survival by Gender**: A count plot showing survival distribution by gender.

These visualizations help in understanding the distribution of important features and their impact on the survival rate.

## Model Training & Evaluation

- **Logistic Regression**: The model used for classification is Logistic Regression, which is a widely used algorithm for binary classification problems.
- **Training and Testing**: The dataset is split into a training set (80%) and a test set (20%) to evaluate the model's performance.
- **Accuracy Evaluation**: The accuracy of the model is evaluated on both the training and test datasets using the accuracy score. The model's performance is evaluated based on how well it predicts survival in both datasets.

### Results:

- **Accuracy on Training Data**: The model’s accuracy when evaluated on the training dataset.
- **Accuracy on Test Data**: The model’s accuracy when evaluated on the test dataset.

## Conclusion

The logistic regression model predicts survival on the Titanic based on passenger data with an acceptable level of accuracy. The key features such as gender, age, class, and embarkation port were crucial in determining the survival outcome. 

Future improvements can involve exploring other machine learning models, such as Random Forest or SVM, and fine-tuning the existing model to improve performance.

## Requirements

- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn