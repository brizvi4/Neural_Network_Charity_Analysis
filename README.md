# Neural Network Charity Analysis

## Overview

In this module, I helped Becks to analyze donations received by corporations from Alphabet Soup. Beks received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Now it is her task to see which of these organizations actually put the money to charitable causes. For this model, we are going to make use of deep-learning neural networks and the TensorFlow framework in Python.

## Results

### Data Preprocessing

- The features for our model are the columns AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, APPLICATION_TYPE, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS and ASK_AMT
- The identity information columns EIN and NAME have been deleted from the input data
- The target variable of the model is the IS_SUCCESSFUL column 

### Compiling, Training, and Evaluating the Model

- The first hidden layer had 43 inputs, 80 neurons and 80 bias terms and the second hidden layer had 80 inputs, 30 neurons and 30 bias terms
- The output layer had 30 inputs (number of neurons from the second hidden layer), 1 neuron, and 1 bias term
- Both the first and second hidden layers were activated using Rectified Linear Unit function while the output layer was activated using the Sigmoid function
- while trying to optimize the model performace, I added one more hidden layer with 10 neurons and I also increased the number of epochs to 200. This only slightly increased the accuracy but did not meet the goal of above 75%
