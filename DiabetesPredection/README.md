# Diabetes Prediction

This project uses machine learning to predict whether a person is diabetic based on several health-related features. We use **Support Vector Machine (SVM)** with a linear kernel for classification and data standardization to improve model accuracy.

## Project Overview

The objective of this project is to predict the likelihood of a person being diabetic based on various medical factors. The model is trained using a dataset that includes features like age, BMI, blood pressure, and more. We use **SVM** as the classification algorithm to predict whether the outcome is diabetic or non-diabetic.

### Features in the Dataset:
- **Pregnancies**: Number of pregnancies
- **Glucose**: Glucose concentration
- **BloodPressure**: Blood pressure value
- **SkinThickness**: Skinfold thickness measurement
- **Insulin**: Insulin levels
- **BMI**: Body Mass Index
- **DiabetesPedigreeFunction**: A function which scores likelihood of diabetes based on family history
- **Age**: Age of the patient
- **Outcome**: The target variable, where:
  - 0 → Non-diabetic
  - 1 → Diabetic

### Requirements

-Python 3.x

-pandas

-numpy

-scikit-learn