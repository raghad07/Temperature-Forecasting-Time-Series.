# Temperature-Forecasting-Time-Series.
#Temperature Forecasting using Time Series Analysis
This repository contains code for temperature forecasting using time series analysis. The goal is to predict the average temperature in Madrid, Spain based on historical temperature data.

#Dataset
The dataset used for this project is the "Daily Temperature of Major Cities" dataset, which provides daily average temperature records for various cities around the world. We have extracted the data for Madrid, Spain from the dataset.

#Data Preparation
Filtered the dataset to include only the data for Madrid, Spain.
Removed unnecessary columns.
Normalized the data using standard scaling.
Plotted histograms to visualize the data distribution before and after normalization.

#Time Series Data Generation
Created a time series dataset using the TensorFlow TimeSeriesGenerator, with a sequence length of 7 (past 7 days' temperatures) and a batch size of 32.

#Model Creation
#Model 1:
Created a convolutional neural network (CNN) model with a bidirectional LSTM layer.
Used the Huber loss function and Adam optimizer for training.

#Model 2:
Created a CNN-GRU model with two GRU layers.
Used the Huber loss function and Adam optimizer for training.

#Training and Evaluation
Trained both models on the prepared dataset.
Evaluated the models using a validation set.
Plotted the true temperature values and predicted temperature values for the last 100 days to visualize the model's performance.

#Results
Model 1 achieved a validation loss of X.
Model 2 achieved a validation loss of Y.

