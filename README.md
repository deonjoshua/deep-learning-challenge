# Building a neural network model to help nonprofit foundation Alphabet Soup select the applicants for funding with the best chance of success in their ventures

## Overview

The purpose of this analysis is to create a deep learning neural network model to predict if an organization funded by Alphabet Soup will be successful or not in their venture. The model is trained using a dataset of over 34,000 organizations that have received funding from Alphabet Soup  over the years.

## Results

### Data Preprocessing

- The target variable for the model is 'IS_SUCCESSFUL'.
- The feature variables for the model are 'APPLICATION_TYPE', 'AFFILIATION', 'CLASSIFICATION', 'USE_CASE', 'ORGANIZATION', 'STATUS', 'INCOME_AMT', 'SPECIAL_CONSIDERATIONS', and 'ASK_AMT'.
- The 'EIN' and 'NAME' columns were removed from the input data because they are neither targets nor features.

### Compiling, Training, and Evaluating the Model

- I initially selected a model with 2 hidden layers with 60 and 20 neurons respectively. The activation function relu was applied to both layers. The output layer had a sigmoid activation function for binary classification. The accuracy of this model was 0.5320
- I was not able to achieve the target performance. 
- I then attempted to increase model performance by increasing the number of neurons, adding another hidden layer, changing the activation function applied to the hidden layers and increasing the number of epochs used to train the model. 
- Despite my efforts the accuracy of the model didn't surpass an accuracy of 0.5320 and was stuck at this value. I am yet to determine if it was an issue with tensorflow on my machine. 

## Summary

The deep learning neural network model did not achieve the desired performance accuracy in predicting the success of Alphabet Soup-funded organizations. Several attempts were made to increase the performance of the model but there was no success. You could train a random forest model to make predictions using this dataset as they are relatively easy to interpret and less computationally expensive than deep learning models.