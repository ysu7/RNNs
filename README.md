# Exploring Recurrent Neural Networks (RNNs) with PyTorch
A. Objective <br>
The objective of this project is to gain hands-on experience with Recurrent Neural Networks (RNNs) using PyTorch. We implement and train an RNN model to perform a specific task and explore its capabilities in sequence modeling.
Begin by researching the fundamentals of RNNs, their architecture, and applications in various fields such as natural language processing, time series analysis, and speech recognition. Familiarize yourself with PyTorch, a popular deep learning framework. <br>
B. Tasks <br>
Setup Environment:We will work on Jupyter Notebook of Google Colab. First of all, we need to decide our research approach and data selection. We will pick up the data, a stock price of time series, because this kind of analyzing is popular in RNNs and the data is easy to access and stable. <br>
Dataset Selection: We will pick up some stock data to analyze the relationships. We will utilize importing yfinance library into Python code directly. yfinance is a popular open source library developed by Yahoo. Through this method, we can fetch the standard stock data with a start time and end time. We pick up the stock price of microsoft from 1995-1-1 to 2020-1-1 as our data, and drop the useless columns, because usually the stock type of data is consisted with 6 parts which are: Open, High, Low, Adj Close, Volume, Close. We only keep close price. <br>
Data Preprocessing:
We created sequences of historical data by the number of days passed on the DataFrame.
This basically means that we converted the original dataset to time series dataset. Inside each one of our time series dataset, it includes all the data of certain time period.
The data choose is :current index + timeline -1. After a series of data cleaning, we convert the data into numpy arrays and split it into training and test sets. The split size is set to 30% which means 30 percent of data for trainning and 70 percent of data for testing. X are used for input features and y used as output features. <br>
Model Implementation:  Design the model architecture, including the input/output dimensions, hidden layer size, activation functions, etc. This is a basic LSTM (Long Short-Term Memory) model using PyTorch (nn.Module).
In the training, We tried experiment with different hyperparameters (learning rate, batch size, epochs, time sequences, number of hidden layers) to optimize the performance of your model.<br>
Analyze the results of the trained RNN model. Interpret its performance on the chosen task and identify any areas for improvement or further experimentation. Explore the model's predictions and understand its behavior in different scenarios.
