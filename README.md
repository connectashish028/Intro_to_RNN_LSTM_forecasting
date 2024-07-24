# Intro_to_RNN_LSTM_forecasting

# Temperature Forecasting using LSTM

This repository contains a Jupyter Notebook that demonstrates how to build a temperature forecasting model using Long Short-Term Memory (LSTM) networks.

## Dataset

The Jena Climate dataset is used for this project. It contains 14 different features (such as air temperature, atmospheric pressure, humidity, wind direction, etc.) recorded every 10 minutes, over several years.  For this model, only the temperature feature is considered.

Link to the dataset: https://www.kaggle.com/datasets/mnassrib/jena-climate/data

## Model Architecture

The model consists of the following layers:

* **Input Layer:** Takes a sequence of 5 temperature values as input.
* **LSTM Layer:** 64 LSTM units.
* **Dense Layer:** 8 neurons with ReLU activation function.
* **Output Layer:** 1 neuron with linear activation function to predict the temperature.

## Training

* The dataset is split into training, validation, and test sets.
* The model is trained using the Adam optimizer with a learning rate of 0.0001.
* The Mean Squared Error (MSE) is used as the loss function and Root Mean Squared Error (RMSE) is used as a metric.
* A ModelCheckpoint callback is used to save the best model based on validation loss.

## Evaluation

* The model is evaluated on the test set using RMSE.

## Results

* The model achieves a good performance on the test set with a low RMSE.

## How to Use

1. Clone the repository.
2. Open the Jupyter Notebook in Google Colab.
3. Run the cells to train and evaluate the model.

## Requirements

* TensorFlow
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
