# Bulldozer Price Prediction

This repository contains an end-to-end machine learning project aimed at predicting the sale prices of bulldozers at auction. The project is a submission to the [Bluebook for Bulldozers](https://www.kaggle.com/competitions/bluebook-for-bulldozers/overview) competition hosted on Kaggle.

The objective of the competition is to predict the auction sale price of heavy equipment based on factors such as usage, equipment type, and configuration. This project applies various machine learning techniques to build a predictive model for this task.

## Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Notebook Breakdown](#notebook-breakdown)
- [Evaluation](#evaluation)

## Overview
The **Bluebook for Bulldozers** competition challenges participants to predict the auction sale price of bulldozers and other heavy equipment. The dataset is sourced from auction results and includes features related to equipment usage, type, and configuration.

The key steps in this project include:
- Data cleaning and preprocessing
- Exploratory data analysis (EDA)
- Feature engineering
- Model building and evaluation
- Hyperparameter tuning for optimal performance

The final model is evaluated using **Root Mean Squared Log Error (RMSLE)**, the competition's chosen metric, which penalizes large errors between predicted and actual sale prices more heavily.

## Dataset
The dataset used in this project is provided by the Kaggle competition [Bluebook for Bulldozers](https://www.kaggle.com/competitions/bluebook-for-bulldozers/data). It consists of historical auction results, including equipment specifications and sale price.

## Notebook Breakdown
This notebook End-to-End Bulldozer-Price-Regression.ipynb details the complete implementation of the project. Here is a high-level overview of the workflow:

1. Data Loading: Load the training and validation datasets.
2. Exploratory Data Analysis (EDA): Perform data visualization and explore key features.
3. Data Cleaning: Handle missing data, perform date parsing, and convert data types.
4. Feature Engineering: Create additional features to enhance model performance based on domain knowledge and insights from EDA.
5. Modeling: Use machine learning models like RandomForest to predict auction prices.
6. Evaluation: Evaluate model performance using RMSLE.
7. Hyperparameter Tuning: Optimize model parameters using techniques like RandomizedSearchCV.

## Evaluation
The model performance is measured using Root Mean Squared Log Error (RMSLE), which captures the differences between the actual and predicted auction prices. 
RMSLE achieved: 24.67 
