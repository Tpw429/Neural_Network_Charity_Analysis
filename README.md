# Neural_Network_Charity_Analysis

## Overview of the Analysis

From Alphabet Soup’s business team, Beks received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as the following:

EIN and NAME - Identification columns <br/>
APPLICATION_TYPE - Alphabet Soup application type <br/>
AFFILIATION - Affiliated sector of industry <br/>
CLASSIFICATION - Government organization classification <br/>
USE_CASE - Use case for funding <br/>
ORGANIZATION - Organization type <br/>
STATUS - Active status <br/>
INCOME_AMT - Income classification <br/>
SPECIAL_CONSIDERATIONS - Special consideration for application <br/>
ASK_AMT - Funding amount requested <br/>
IS_SUCCESSFUL - Was the money used effectively <br/>

We'll use the features in the provided dataset to help Beks create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. In this project, I preformed an ETL (Extract, Tranfer, and Load) process on the data, which I then used to train and test to create predictions using neural networks to find which charities should receive funding. The accuracy was measured to see how successful the prediction was for each of the charities.

## Results

* Data Preprocessing
  * What variable(s) are considered the target(s) for your model? The 'IS_SUCCESSFUL' column.
  * What variable(s) are considered to be the features for your model? The features are 'APPLICATION_TYPE', 'CLASSIFICATION', 'USE_CASE', 'ORGANIZATION', 'STATUS', 'INCOME_AMT', 'SPECIAL_CONSIDERATIONS', and 'ASK_AMT'.
  * What variable(s) are neither targets nor features, and should be removed from the input data? 'EIN' and 'NAME' are the two variables that should be removed.

* Compiling, Training, and Evaluating the Model
  * How many neurons, layers, and activation functions did you select for your neural network model, and why? Two hidden layers with the following neurons for each layer: hidden_nodes_layer1 = 24. hidden_nodes_layer2 = 12. These were picked to achieve higher accuracy.
  * Were you able to achieve the target model performance? After optimizing my model, I was able to bring my accuracy up to nearly 75%.
  * What steps did you take to try and increase model performance? Adding hidden layers, adding neurons, and changing the activation function with callback.

## Summary
The deep learning model is superior in terms of accuracy when compared to different models. The accuracy increased the most when the activation was changed with callback. One recommendation I have to solve the classification problem is to consider using the RandomForestClassifier model, because it can handle tabular data very well and use a number of weak learners to predict the classification beased on all the learners, thus increasing model accuracy.

