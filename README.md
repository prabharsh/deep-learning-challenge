# deep-learning-challenge
deep-learning-challenge
# Deep Learning Challenge

## Background
The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team, you have received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as:

EIN and NAME—Identification columns
APPLICATION_TYPE—Alphabet Soup application type
AFFILIATION—Affiliated sector of industry
CLASSIFICATION—Government organization classification
USE_CASE—Use case for funding
ORGANIZATION—Organization type
STATUS—Active status
INCOME_AMT—Income classification
SPECIAL_CONSIDERATIONS—Special considerations for application
ASK_AMT—Funding amount requested
IS_SUCCESSFUL—Was the money used effectively

## Neural Network Model Report
1. Overview of the analysis: Explain the purpose of this analysis.
-  The purpose of this analysis is to evaluate if an Alphabet Soup-funded organization will succeed based on the features in the dataset. 

2. Data Preprocessing
    - What variable(s) are the target(s) for your model?
        - The model goal is column 'IS_SUCCESSFUL' 
    - What variable(s) are the features for your model?
        - The structure of the model include APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, INCOME_AMT, and SPECIAL_CONSIDERATIONS. These are displayed after the removal of unwanted  columns 'EIN' and 'NAME'.
    - What variable(s) should be removed from the input data because they are neither targets nor features?
        - STATUS and SPECIAL_CONSIDERATIONS should be removed from the data as in the 'STATUS' column they were the same value - 1 for Status, and SPECIAL_CONSIDERATONS have no numerical data. 
* Compiling, Training, and Evaluating the Model
    - How many neurons, layers, and activation functions did you select for your neural network model, and why?
        - In the first attempt, with Layer 1 at 8 and Layer 2 at 5 and activation functions = relu, Loss: 0.55, Accuracy: 0.7263.
            - Reference: Image01.png in Images.
    - Were you able to achieve the target model performance?
        - No, Although the target model performance was not achieved, 72.5%. accuracy was  accomplished 
    - What steps did you take in your attempts to increase model performance?
        - Model performance was upscaled by amplifying the hidden layers and also by alternating activation functions from relu to segmoid.
            - Reference: Image02.png and Image03.png

* Summary: 
75% accuracy was achieved through the deep learning model results. 
Removing additional and non quantifiable columns from data frame would not take up space. 
Changing the activation functions increases accuracy to 75% accuracy. 
Trimming a neural network will determine an optimal structure for a neutral network.



