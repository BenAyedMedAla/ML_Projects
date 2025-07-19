# Car Price Prediction

This project aims to predict the selling price of cars based on various features such as the car's fuel type, seller type, transmission, and other features. We use **Linear Regression** and **Lasso Regression** models to make the price predictions.

## Project Overview

The goal of this project is to predict the selling price of used cars based on various attributes. We explore different machine learning models, including **Linear Regression** and **Lasso Regression**, to assess which model gives the best predictions for car prices.

### Features in the Dataset:
- **Car_Name**: The name of the car (not used in the prediction model)
- **Fuel_Type**: The fuel type of the car (Petrol, Diesel, CNG)
- **Seller_Type**: The type of seller (Dealer or Individual)
- **Transmission**: The transmission type of the car (Manual or Automatic)
- **Owner**: The number of previous owners
- **Year**: The year of manufacture
- **Kms_Driven**: The number of kilometers driven
- **Engine**: The engine capacity of the car
- **Power**: The power of the car
- **Mileage**: The mileage of the car
- **Seats**: The number of seats in the car
- **Selling_Price**: The target variable, which is the selling price of the car

### RQ: 
Both Linear Regression and Lasso Regression models provide good predictions for car prices, but the R-squared error for the models can be further optimized. Lasso Regression provides a regularization mechanism that may help in improving the model's generalization. Future work could involve hyperparameter tuning or trying other regression techniques.

### Requirements
-Python 3.x

-pandas

-numpy

-matplotlib

-seaborn

-scikit-learn