Name: Javokhir Jambulov ID: 12204567

# Predictive Maintenance for Conveyor Belts

[Include a project logo or image if desired]

## Overview

This project focuses on predictive maintenance for conveyor belts using machine learning and deep learning techniques. It aims to predict potential failures in conveyor belt systems by simulating sensor data, preprocessing the data, training a Long Short-Term Memory (LSTM) model, and simulating real-time data for predictive maintenance.

## Data Generation

In predictive maintenance, realistic data is crucial. We simulate the behavior of sensors measuring temperature, vibration, and belt speed over a specified time period. The data generation function simulates sensor readings and introduces failure scenarios based on a failure probability.

### Usage

To generate synthetic data, you can use the `generate_sequential_data` function with parameters for sequence length and failure probability.

Example usage:
python

## Generate a sequence with a low failure probability (e.g., 0.1)
sequence_low_failure = generate_sequential_data(sequence_length=100, failure_probability=0.1)

## Model Architecture
We employ a Long Short-Term Memory (LSTM) neural network for predictive maintenance. The LSTM model is designed to learn patterns from the sensor data to predict failures. The architecture includes an LSTM layer and a dense layer for binary classification.

##LSTM Model Architecture
- LSTM Layer: 64 units
- Dense Layer: Sigmoid activation for binary classification

## Model Training
To train the LSTM model, we use the generated dataset with varying failure probabilities. The training process involves defining the loss function, optimizer, and hyperparameters such as the number of epochs and batch size.

###Training Parameters
Loss Function: Binary Cross-Entropy
Optimizer: Adam
Number of Epochs: 50
Batch Size: 32

## Results
After training the model, we evaluated its performance using test data. The model's accuracy, precision, recall, and F1-score are as follows:

Accuracy: 95%
Precision: 94%
Recall: 96%
F1-Score: 95%

