# Neural_Network_Charity_Analysis

## Overview of the Analysis

The purpose of this project was to create a binary classifier to predict if non-profit applicants will be successful if funded by Alphabet Soup. The dataset contained over 34,000 organizations and information pertaining to their funding history, income, status, and if they were successful or not. The main objective was to preprocess the data, compile, train, and evaluate a neural network model and then optimize it for 75% or higher accuracy. 

    Resources
        - Data Sources: charity_data.csv
        - Software: Python, Pandas, tensorflow, sklearn, Jupyter Notebook

## Results

#### Data Preprocessing

What variable(s) are considered the target(s) for your model?
- The target variable for this model was the "IS_SUCCESSFUL" variable. 
    
What variable(s) are considered to be the features for your model?
- The features for this model are 'APPLICATION_TYPE','AFFILIATION', 'CLASSIFICATION','USE_CASE','ORGANIZATION','STATUS','INCOME_AMT','SPECIAL_CONSIDERATIONS', and 'ASK_AMT'. 
    
What variable(s) are neither targets nor features, and should be removed from the input data?
- The variables that were neither targets nor features and were removed from the input data are the non-beneficial ID columns; "EIN" and "NAME".

#### Compiling, Training, and Evaluating the Model

How many neurons, layers, and activation functions did you select for your neural network model, and why?
- In the original model, prior to optimization, I selected 2 hidden layers with 80 and 30 neurons respectively. Both hidden layers used the ReLU activation function and the output layer used the sigmoid activation function because they matched the complexity of the input data.  

Were you able to achieve the target model performance?
- **I was unable to reach the target model performance**. The closest to the target (75%) was **72.7% accuracy** with my original model. 

What steps did you take to try and increase model performance?
- In attempts to optimize my models performance, I added additional neurons to hidden layers, added new hidden layers, and changed the optimization function on the hidden layers. See results below.

***Below are the results of the original model and all 3 optimization attempts made.***

1. **Original Model** 
    - Model Layout:
    
    ![alt text](https://github.com/coconnell022/Neural_Network_Charity_Analysis/blob/main/Images/Original%20Layout.png?raw=true)

    - Evaluation Results:
    
    ![alt text](https://github.com/coconnell022/Neural_Network_Charity_Analysis/blob/main/Images/Original%20Results.png?raw=true)

2. **Optimization Attempt 1: Adding an additional hidden layer**
    - Model Layout:
    
    ![alt text](https://github.com/coconnell022/Neural_Network_Charity_Analysis/blob/main/Images/1%20Layout.png?raw=true)

    - Evaluation Results:
    
    ![alt text](https://github.com/coconnell022/Neural_Network_Charity_Analysis/blob/main/Images/1%20Results.png?raw=true)

3. **Optimization Attempt 2: Adding more neurons in hidden layers**
    - Model Layout:
    
    ![alt text](https://github.com/coconnell022/Neural_Network_Charity_Analysis/blob/main/Images/2%20Layout.png?raw=true)

    - Evaluation Results:
    
    ![alt text](https://github.com/coconnell022/Neural_Network_Charity_Analysis/blob/main/Images/2%20Results.png?raw=true)

4. **Optimization Attempt 3: Changing the activation function of hidden layers**
    - Model Layout:
    
    ![alt text](https://github.com/coconnell022/Neural_Network_Charity_Analysis/blob/main/Images/3%20Layout.png?raw=true)

    - Evaluation Results:
    
    ![alt text](https://github.com/coconnell022/Neural_Network_Charity_Analysis/blob/main/Images/3%20Results.png?raw=true)



## Summary

Overall, **the optimization attempts to reach a 75% or higher accuracy was not accomplished**. The closest accuracy of 72.7% was achieved using the original model, prior to any optimization attempts. The first attempt added an additional hidden layer that allows neurons to train on activated input values which can identify nonlinear characteristics without needing more data. The second attempt of adding more neurons in the hidden layers had a diminishing effect by lowering the accuracy from the original model. The third attempt made changed the activation function of the hidden layers to a higher complexity activation function which assessed the data without risk of ignoring lower complexity features.

**A recommendation for how a different model could solve this classification problem would be to use a Random Forest model** to handle the large dataset for a potential of higher optimization. Another recommendation would be to increase the number of epochs to the training regimen. This would allow more information to be provided to each neuron from the input data which would apply more effective weight coefficients. However, like many optimizing and fine-tuning attempts, this method has the potential to lead to overfitting. 


        Caroline O'Connell
        February 21st, 2021
