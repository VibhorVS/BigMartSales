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
