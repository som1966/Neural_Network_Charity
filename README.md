# Neural_Network_Charity

## Overview
Alphabet Soup Company has requested the team to analyze 34,000 organizations and their measures to predict which should be funded.  For the analysis, Machine Learning and Neural Network models will used to predict the organizations. The steps to be completed are:

 1) Processing the data for Neural Networks model

 2) Training and evaluating the model

 3) Optimization for Model.
 
 Resources:
 
 Data File:  charity_csv.
 Software:  Python 3.7.1, Pandas 1.2.4
 
 ## Data Preprocessing
 
 Preprocessing included dropping the variables EIN and Name that were not needed for the analysis.  The features "Application_Type" and "Classification" were preprocessed to create appropriate binning of the contained values.

Application Counts

![image](https://user-images.githubusercontent.com/89953246/149603855-f0c57cbc-6b07-40d9-9681-6a68db71fd5e.png)

Classification Counts

![image](https://user-images.githubusercontent.com/89953246/149603893-35212118-d294-40bd-9dc6-78ddf9c1337b.png)

OneHotEncoder was used and tables were merged.

![image](https://user-images.githubusercontent.com/89953246/149603946-e9a20666-2b89-4022-90a7-1fd42868f306.png)

Preprocessed data was split into features based on "IS_SUCCESSFUL".

![image](https://user-images.githubusercontent.com/89953246/149603994-2388025e-40b8-44ec-8a0d-1d610d8be330.png)

## Compile, Train and Evaluate Model

The original model had two hidden layers with 10 and 5 neurons, respectively.  The Rectified Linear Unit ("relu") was used for both the 1st and 2nd layer; "sigmoid" for the 
output layer. The model achieved 73% accuracy.

![image](https://user-images.githubusercontent.com/89953246/149604124-a0ed71cf-fe44-4fe7-9c25-2247e21d00f0.png)

Three additional models were created to optimize the model and see if accurracy could be increased to 75%.

## Optimization of Model Results

Optimization Model 1 
A 3rd layer was added to the original model with 2 neurons and the activation for that layer was "relu".

![image](https://user-images.githubusercontent.com/89953246/149604325-027932a3-3854-4e6a-918d-6f7465d8d523.png)

Optimization Model 2
Additional neurons (30, 45) were added to the original model's two layers.

![image](https://user-images.githubusercontent.com/89953246/149604386-80284fa8-522a-46bc-b0d8-4edb274986a2.png)

Optimization Model 3
The activation for both hidden layers were changed to "tanh" with output layer changed to "relu".

![image](https://user-images.githubusercontent.com/89953246/149604488-f9596719-1dbe-4b6c-bc68-4f0e7550d254.png)

## Summary
The overall accuracy of the original model and the optimzation models remained at 73%. Further models could be created using the deep learning approach by changing the binning preprocess or continue exploring hidden layers and number of neurons.  Another possibility is to complare current resuls with Logistic Regression or RandomForest model. 
