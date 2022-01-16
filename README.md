# Neural Network Analysis

## Overview of Project
An analysis of Charity funding data using machine learning neural network model

### Purpose
The purpose of this analysis is to clean data using python and pandas, create a neural network, input the data and attempt at optimizing the machine learning model

## Analysis and Results

### Data Preprocessing
- Values that are considered features for the model: APPLICATION_TYPE AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, ASK_AMT, SPECIAL_CONSIDERATIONS
- Unsure if STATUS is a useful metric

- Values that are considered targets fir the model: IS_SUCCESSFUL

- Values to be removed: EIN, NAME

### Compiling, Training, Evaluating
- 3 Hidden layers were chosen to attempt to use 3 different activation functions, makes the model prone to overfitting but accuracy wass still very low
- Sigmoid, Relu, and tanh activation functions were used to try to find different trends within the data that may not be linear

- Unsuccessful in reaching target performance

Steps taken to icrease accuracy

- Removed any rows that were considered "special considerations" as they could skew data
- Removed any rows with an asking amount of over 99 million as there were large outliers in the data
- Added a new hidden layer
- Changed activation function of all hidden layers
- Changed number of neurons in each layer
- Increased number of epochs

## Summary
Overall the results after cleaning the data further and attempting to fit the data to the model greatly decreased the accuracy. The model ended at only 56% accuracy after many tweaks. 
There must be some kind of outliers in the data or missing information that would explain why a charity was successful or not.
I am not sure that a different model would have any better accuracy in this scenario, but a vector model may prove to have better accuracy as it seperates linearly seperable data well