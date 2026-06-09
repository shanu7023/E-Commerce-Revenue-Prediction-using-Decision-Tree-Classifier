# E-Commerce Revenue Prediction

## Overview

This project builds a machine learning model to predict whether an e-commerce customer session will result in a purchase (Revenue = 1) or not (Revenue = 0).

The workflow includes:

* Data preprocessing using Scikit-learn Pipelines
* Numerical feature scaling with StandardScaler
* Categorical feature encoding with OneHotEncoder
* Feature transformation using ColumnTransformer
* Model training using Decision Tree Classifier
* Model evaluation using F1 Score, Classification Report, and Confusion Matrix
* Hyperparameter tuning using GridSearchCV

## Dataset

The dataset used is:

`shop_smart_ecommerce.csv`

### Target Variable

* **Revenue**

  * 1 = Purchase made
  * 0 = No purchase

### Feature Types

* Numerical Features
* Categorical Features

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn

## Project Workflow

### 1. Data Loading

The dataset is loaded using Pandas.

### 2. Data Preprocessing

The features are separated into:

* Numerical columns
* Categorical columns

A preprocessing pipeline is created using:

* StandardScaler for numerical features
* OneHotEncoder for categorical features

### 3. Model Building

A Decision Tree Classifier is trained with:

* max_depth = 6
* min_samples_leaf = 30
* class_weight = "balanced"
* random_state = 42

### 4. Pipeline Creation

A Scikit-learn Pipeline combines:

1. Data preprocessing
2. Model training

This ensures all transformations are applied consistently during training and prediction.

### 5. Model Evaluation

The model performance is evaluated using:

* F1 Score
* Classification Report
* Confusion Matrix

### 6. Hyperparameter Tuning

GridSearchCV is used to find the best combination of:

* max_depth
* min_samples_leaf

using 5-fold cross-validation and F1 score as the optimization metric.

## Results

The project outputs:

* Best F1 Score
* Best Hyperparameters
* Classification Report
* Confusion Matrix

## Folder Structure

```text
├── shop_smart_ecommerce.csv
├── ecommerce_revenue_prediction.ipynb
├── README.md
```


## Learning Outcomes

Through this project, you will learn:

* Data preprocessing using ColumnTransformer
* Building end-to-end ML pipelines
* Handling categorical and numerical features
* Decision Tree classification
* Model evaluation metrics
* Hyperparameter tuning with GridSearchCV

## Future Improvements

* Random Forest Classifier
* XGBoost Classifier
* Feature importance analysis
* Model deployment using Flask or Streamlit
* Advanced feature engineering

## Author

Shanu

Machine Learning | Data Analytics | Python | Scikit-Learn
