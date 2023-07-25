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


