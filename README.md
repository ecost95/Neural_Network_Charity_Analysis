# Neural_Network_Charity_Analysis

## Overview: 
We will be using a machine learning and neural networks to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

We will use a CSV containing more than 34,000 organizations that have received funding. The dataset contains a number of columns that capture metadata about each organization.

## Results: 
## Data Preprocessing:

### What variable(s) are considered the target(s) for our model?
 - The target variable is the column "IS_SUCCESSFUL", which tells us if the money used effectively
 
### What variable(s) are considered to be the features for our model?
The features variables are: 
- APPLICATION_TYPE—Alphabet Soup application type
- AFFILIATION—Affiliated sector of industry
- CLASSIFICATION—Government organization classification
- USE_CASE—Use case for funding
- ORGANIZATION—Organization type
- STATUS—Active status
- INCOME_AMT—Income classification
- SPECIAL_CONSIDERATIONS—Special consideration for application
- ASK_AMT—Funding amount requested

### What variable(s) are neither targets nor features, and should be removed from the input data?
-We removed the EIN and NAME columns, as these are only used for identification and are not useful for our analysis.

## Compiling, Training, and Evaluating the Model:

### How many neurons, layers, and activation functions did we select for your neural network model, and why?
- We chose two include two hidden layers, with 80 neurons and 30 neurons respectively. We chose 80 because the rule of thumb is that neurons should be 2 to 3 times the number of inputs (44 in our case). For the activation function in the hidden layers, we chose to use ReLU, as this function is optimal for positive non-linear input for classification or regression. For the output layer, we chose a Sigmoid activation function, as this is optimized for binary classification.

### Were we able to achieve the target model performance?
- With our first model, target was able to achieve  0.726% accuracy. 

###What steps did we take to try and increase model performance?
- In our optimization file, we tweaked the model to try to improve out accuracy. To do this we:
1) removed the "SPECIAL_CONSIDERATIONS" column from our features
2) added a third hidden layer
3) ran the model for 90 epochs instead of 100

However, we did not see much of a change in accuracy with these changes (0.725%)

## Summary: The deep learning model was somewhat successful for predicting the success of businesses recieving funcding with over 72% accuracy. For future analysis, we would recomend a more robust dataset and using different activation functions.
