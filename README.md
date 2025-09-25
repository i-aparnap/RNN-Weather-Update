# RNN-Weather-Update
# Weather Temperature Prediction using SimpleRNN
## Overview

This project implements a Recurrent Neural Network (RNN) using SimpleRNN to predict the next day’s temperature based on historical weather data. It involves data preprocessing, sequence creation, RNN model building, training, evaluation, and short-term forecasting.

## Dataset

Daily Weather Dataset (Example: Kaggle)

Key Features:

Date

Temperature (target variable)

Humidity

Wind Speed

Pressure (optional)

## Goal: Forecast next day’s temperature using previous 7–14 days of weather data.

## Data Preprocessing

Displayed first 10 rows and plotted temperature trends

Checked and handled missing values (imputation/removal)

Normalized features using MinMaxScaler for faster RNN convergence

Created input sequences using past 7–14 days’ data

Split dataset into train, validation, and test sets

## SimpleRNN Model Architecture

Input layer: shape = sequence length × number of features

SimpleRNN layer: 32–64 units

Optional Dropout layer to prevent overfitting

Dense output layer: 1 unit (linear activation for regression)

Loss function: Mean Squared Error (MSE)

Optimizer: Adam

Metrics: Mean Absolute Error (MAE)

Training Parameters:

Batch size: 32

Epochs: 50–100

Validation data used for performance monitoring

Plotted training vs. validation loss curves

## Model Evaluation & Forecasting

Evaluated model on test data using:

RMSE (Root Mean Squared Error)

MAE (Mean Absolute Error)

R² score

Plotted predicted vs actual temperatures

Forecasted next 7 days temperature and visualized predictions alongside historical data

## How to Run

Open RNN_Assignment.ipynb in Jupyter Notebook or Google Colab

Execute cells sequentially: preprocessing → sequence creation → model training → evaluation → forecasting

## Dependencies

Python 3.8+

TensorFlow / Keras

NumPy

Pandas

Matplotlib

scikit-learn

## Author

Aparna P
