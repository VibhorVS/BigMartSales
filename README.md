# Sales Prediction Model

This repository contains Python code for a sales prediction model using the XGBoost regressor. The model is trained on a dataset containing information about various items and their sales in different outlets.

## Table of Contents
- [Introduction](#introduction)
- [Prerequisites](#prerequisites)
- [Data Preprocessing](#data-preprocessing)
- [Model Training](#model-training)
- [Evaluation](#evaluation)

## Introduction

Sales prediction is a crucial task for businesses to optimize inventory and resources. This repository provides a basic template for building a sales prediction model using XGBoost. The dataset used here contains information about items, outlets, and their corresponding sales.

## Prerequisites

Before you begin, ensure you have met the following requirements:

- Python 3.6+
- Required Python packages: `numpy`, `pandas`, `matplotlib`, `seaborn`, `scikit-learn`, `xgboost`

## Data Preprocessing

The dataset (Train.csv) is loaded and preprocessed in the following steps:

- Missing values in the 'Item_Weight' column are filled with the mean value.
- Missing values in the 'Outlet_Size' column are filled with the mode value based on the 'Outlet_Type'.
- Data visualization using seaborn to understand the distributions and relationships between features.
- Encoding categorical variables using LabelEncoder.

## Model Training

The model for sales prediction is trained using the XGBoost regressor, a powerful machine learning algorithm known for its efficiency in handling structured data and providing accurate predictions.

### Data Splitting

Before training the model, the dataset is divided into two subsets: the training set and the testing set. This is done to evaluate the model's performance on unseen data. The `train_test_split` function from `scikit-learn` is used for this purpose. By default, 80% of the data is used for training, and 20% is reserved for testing. You can adjust the split ratio as needed.

```python
X_train, X_test, Y_train, Y_test = train_test_split(X, Y, test_size=0.2, random_state=2)
```

## Model Selection and Training
The XGBoost regressor is chosen as the model for this task due to its capability to handle regression problems effectively. It is an ensemble learning method that combines the predictions from multiple decision trees.
