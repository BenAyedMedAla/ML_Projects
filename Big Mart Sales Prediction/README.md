# Big Mart Sales Prediction

This project aims to predict the sales of items in Big Mart stores based on various features such as item details, outlet characteristics, and other factors. The model uses **XGBoost Regressor** to predict the sales and evaluates the model’s performance based on R-squared values.

## Project Overview

The goal of this project is to create a predictive model that estimates the sales of items at Big Mart stores using various features. We perform data preprocessing, handle missing values, and apply machine learning techniques to train a model for sales prediction.

The key steps involved are:

1. **Data Collection & Processing**: Loading the dataset and handling missing values and categorical features.
2. **Exploratory Data Analysis (EDA)**: Analyzing the distribution of numerical and categorical features.
3. **Data Preprocessing**: Handling missing values, encoding categorical features, and splitting data into features and target.
4. **Model Training**: Using **XGBoost Regressor** to predict item outlet sales.
5. **Model Evaluation**: Evaluating the model performance using R-squared values.

## Dataset

The dataset consists of the following key features:

### Numerical Features:
- **Item_Weight**: Weight of the item.
- **Item_Visibility**: The visibility of the item in the store.
- **Item_MRP**: Maximum Retail Price of the item.
- **Item_Outlet_Sales**: The sales of the item at the outlet (target variable).
- **Outlet_Establishment_Year**: The year in which the outlet was established.

### Categorical Features:
- **Item_Identifier**: Unique identifier for each item.
- **Item_Fat_Content**: Whether the item is fat or low-fat.
- **Item_Type**: Type of the item (e.g., Snacks, Beverages).
- **Outlet_Identifier**: Unique identifier for each outlet.
- **Outlet_Size**: Size of the outlet (e.g., Small, Medium, Large).
- **Outlet_Location_Type**: The location of the outlet (e.g., Tier 1, Tier 2, Tier 3).
- **Outlet_Type**: Type of outlet (e.g., Grocery, Supermarket).

### Missing Values:
- Missing values were handled by filling them with appropriate statistics like the mean or mode of the column.

### Target Variable:
- **Item_Outlet_Sales**: The target variable that we aim to predict.

## Data Preprocessing

- **Handling Missing Values**: 
  - Missing values in numerical columns like `Item_Weight` were filled with the mean value of the respective column.
  - Missing values in categorical columns like `Outlet_Size` were filled with the mode value, calculated by the type of outlet.

- **Label Encoding**: 
  - Categorical features were converted to numerical values using **Label Encoding**, including columns like `Item_Identifier`, `Item_Fat_Content`, `Item_Type`, `Outlet_Identifier`, `Outlet_Size`, `Outlet_Location_Type`, and `Outlet_Type`.

## Model Training

- **XGBoost Regressor**: The model used for prediction is **XGBoost Regressor**, a powerful machine learning algorithm that works well for regression tasks.
- The model was trained using the training dataset (`X_train` and `Y_train`).

## Model Evaluation

- **R-squared Value**: The R-squared value was used to evaluate the performance of the model. This value indicates how well the model is able to explain the variance in the target variable.
- The model was evaluated on both the training and test datasets (`X_train`, `X_test`, `Y_train`, and `Y_test`).

## Key Features and Insights

- **Item_Weight**: Heavier items tend to have a higher sales volume.
- **Item_Visibility**: Items with higher visibility have better sales performance.
- **Item_MRP**: The price of the item plays a key role in predicting sales.
- **Outlet_Type**: Different outlet types (e.g., Supermarkets vs. Grocery stores) influence sales differently.
- **Outlet_Location_Type**: The outlet's location in a tiered city system (e.g., Tier 1, Tier 2, Tier 3) impacts sales.

## Results

- The model was evaluated using R-squared values, which were calculated for both the training and test datasets.
- The model achieved an **R-squared value** for the training data and test data that indicates the accuracy of predictions.

## Requirements

- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- xgboost
