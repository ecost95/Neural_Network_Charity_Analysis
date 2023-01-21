# Neural_Network_Charity_Analysis

## Overview: 
We will be using a machine learning and neural networks to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

We will use a CSV containing more than 34,000 organizations that have received funding. The dataset contains a number of columns that capture metadata about each organization.

## Results: 
# Data Preprocessing
We categorized our data into "features" and "traget" dataframes:

1) What variable(s) are considered the target(s) for your model?
 - The target variable is the column "IS_SUCCESSFUL", which tells us if the money used effectively

2) What variable(s) are considered to be the features for your model?
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

3) What variable(s) are neither targets nor features, and should be removed from the input data?
-We removed the EIN and NAME columns, as these are only used for identification and are not useful for our analysis.

# Compiling, Training, and Evaluating the Model
1) How many neurons, layers, and activation functions did you select for your neural network model, and why?
- We chose 
Were you able to achieve the target model performance?
- The target was able to achieve  0.726% accuracy. 

What steps did you take to try and increase model performance?
- In our optimization file, we 
