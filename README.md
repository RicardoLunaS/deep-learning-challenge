# deep-learning-challenge


## Overview
The nonprofit foundation Alphabet Soup needs a tool that can help select the applicants for funding with the best chance of success in their ventures considering the historical data from past fundings. A deep learning neural network will be used to predict the result of an applicant.

## Results

### Data preprocessing
The current available relevant data from past fundings include: 
1) Affiliated sector of industry
2) Government organization classification
3) Use case for funding
4) Organization type
5) Active status
6) Income classification
7) Special considerations for application
8) Funding amount requested
9) Was the money used effectively or was the funding successful.

The target variable was variable 9, while variables 1-8, were used as features to predict.

From the feature variables, some can be removed as they do not help predict the success of the funding. These variables were: 
1) Active Status
2) Special Considerations for application
3) Organization type


### Compiling, Training, and Evaluating the Model


How many neurons, layers, and activation functions did you select for your neural network model, and why?
Different modelations were run to reach at least a 75% of the accuracy of the model:

Model 1: 3 hidden layers, with 80, 60 and 35 neurons respectively. Activation functions were Rectified Linear Unit, Hyperbolic Tangent, Rectified Linear Unit and Sigmoid.
Model 2: 3 hidden layers, with 50, 40, and 35 neurons respectively. Activation functions were Rectified Linear Unit, Sigmoid, Rectified Linear Unit and Sigmoid.
Model 3: 2 hidden layers, with 90, 50 neurons respectively. Activation functions were Rectified Linear Unit, Sigmoid.

Target model performance was not achieved, with 73% in all three models.

What steps did you take in your attempts to increase model performance?
Change activation functions, quantity of neurons, columns were dropped such as Status, Special Considerations an Organization Type, small count for application type and classification bins were also modified to increase the category of "Others".

## Summary: 

Three Deep Learning models were run with a 73% accuracy to predict if a funding application is going to be successful depending on the application characteristics.
The models did achieve the minimum target of 75% so other models should be used to solve this classification problem such as Logistic Regression, SVM or Random Forest.

