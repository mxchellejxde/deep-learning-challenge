# Deep Learning Challenge - Alphabet Soup Charity

## Background/Overview

The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With the knowledge of machine learning and neural networks, features in the provided dataset will be used to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team, a CSV will be received containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as:

  1. `EIN` and `NAME` — Identification columns
  2. `APPLICATION_TYPE` — Alphabet Soup application type
  3. `AFFILIATION`— Affiliated sector of industry
  4. `CLASSIFICATION` — Government organization classification
  5. `USE_CASE` — Use case for funding
  6. `ORGANIZATION` — Organization type
  7. `STATUS` — Active status
  8. `INCOME_AMT` — Income classification
  9. `SPECIAL_CONSIDERATIONS` — Special considerations for application
  10. `ASK_AMT` — Funding amount requested
  11. `IS_SUCCESSFUL` — Was the money used effectively

## Process

### Preprocess the Data
In order to design a neural network, the initial step is to preprocess the data. This is a crucial step in the data preparation before feeding it into the a machine learning model. Its purpose is to transform the raw data into a format that is more suitable and useful for the learning algorithms. Part of the preprocessing includes data cleaning (ie removing columns, removing missing values), normalization/scaling (prevent the outliers to overpower data), splitting into training and testing sets, handling categorical data (get dummies).

### Compile, Train, and Evaluate the Model
At this point of the process, a neural network model is created. Here, the input features/nodes for each layer is selected. Hidden layers and output layers with appropriate activation functions are created. Then, the model is compiled and trained, calculating the loss and accuracy with the test data. 

### Model Optimization
To optimize the model to achieve a target predictive accuracy that is higher than 75%, different methods can be utilized. Some ways to adjust the input data to ensure that no variables or outliers are causing confusion in the model -
  1. Dropping more or fewer columns.
  2. Creating more bins for rare occurrences in columns.
  3. Increasing or decreasing the number of values for each bin.
  4. Add more neurons to a hidden layer.
  5. Add more hidden layers.
  6. Use different activation functions for the hidden layers.
  7. Add or reduce the number of epochs to the training regimen.

## Results
The first compiling, training and evaluating of the model had an accuracy of 72.78% and loss of 55.94%. The optimization brought the accuracy to 77.94% and a loss of 45.88%. This is due to an added layer, new activation functions, added column in the preprocessing data, etc. With a logisitic regression model, we could limit the variables and as such provide a better explanation of the data, yet the accuracy may be much lower. A classification report may be used to test changes in performance.

## Summary

#### Data Preprocessing:
  1. Target Variable: `IS_SUCCECSSFUL`
  2. Feature Variables:
      a. `APPLICATION_TYPE`
      b. `AFFILIATION`
      c. `CLASSIFICATION`
      d. `USE_CASE`
      e. `ORGANIZATION`
      f. `STATUS`
      g. `INCOME_AMT`
      h. `SPECIAL CONSIDERATIONS`
      i. `ASK_AMT`
  3. Unused Parameters:
      a. `EIN`
      b. `NAME` - recovered for optimization process

#### Alphabet Soup Charity Details:
Hyperparameters: 
    1. 2 hidden layers
    2. 1st hidden layer: 
        - 80 neurons
        - activation function: "relu"
    3. 2nd hidden layer: 
        - 30 neurons
        - activation function: "relu"
    4. epochs: 100
Accuracy: 72.78%
Loss: 55.94%

![Model 1 Image](images/Model1AccuracyResult.png)

#### Optimization of Alphabet Soup Charity Details:
Hyperparameters: 
    1. 3 hidden layers
    2. 1st hidden layer: 
        - 10 neurons
        - activation function: "relu"
    3. 2nd hidden layer: 
        - 20 neurons
        - activation function: "relu"
    4. 3rd hidden layer: 
        - 30 neurons
        - activation function: "relu"
    5. epochs: 100
Accuracy: 77.94%
Loss: 45.88%

![Model 2 Image](images/Model2AccuracyResult.png)

