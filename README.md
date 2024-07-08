Stock Price Prediction Using LSTM Neural Networks

Overview

# LSTM_AAPL_Stock_Prediction
This repository contains code for predicting Apple Inc. (AAPL) stock prices using an LSTM neural network. It covers data preprocessing, model building, and visualization, accounting for stock changes from the launch of the first iPhone to the present.

Project Structure
Data Fetching and Preprocessing

Historical data from Yahoo Finance is fetched using yfinance.
Data preprocessing includes scaling using MinMaxScaler and sequence generation for LSTM.
Model Architecture

Implemented LSTM layers with dropout for regularization.
Configured the model with Adam optimizer and mean squared error loss.
Training

Trained the model on 80% of the data, with 100 epochs.
Evaluation

Evaluated the model performance using Mean Absolute Error (MAE), Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and R-squared (R2 score).
Visualization

Visualized original vs. predicted stock prices over time.
Files Included
main.py: Python script containing the complete pipeline from data fetching to model evaluation and visualization.
my_model.keras: Saved model file after training.
Requirements
Python 3.x
Libraries: pandas, matplotlib, yfinance, numpy, tensorflow, scikit-learn
Instructions
Setup Environment

Install Python dependencies: pip install -r requirements.txt
Run the Code

Modify start_date_str in main.py to change the historical data fetching start date.
Execute python main.py to fetch data, train the model, and generate predictions.
Interpreting Results

After running, observe the plots generated to visualize predicted vs. actual stock prices.
Check the console for evaluation metrics (MAE, MSE, RMSE, R2 score).
Notes
Adjust model architecture (e.g., number of LSTM layers, units, dropout rates) based on specific needs and data characteristics.
Experiment with different stocks or time periods by modifying the ticker and start_date_str parameters in main.py
