# Neural_Network_Charity_Analysis

## Overview of the Analysis

The purpose of this project 

    Resources
        - Data Sources: charity_data.csv
        - Software: Python, Pandas, sklearn, Jupyter Notebook

## Results

#### Data Preprocessing

What variable(s) are considered the target(s) for your model?
- The target variable for this model was the "IS_SUCCESSFUL" variable with a value of "1" that represents "True" or "Yes". 
    
What variable(s) are considered to be the features for your model?
- The features for this model are the categorical variables such as 'APPLICATION_TYPE','AFFILIATION', 'CLASSIFICATION','USE_CASE','ORGANIZATION','INCOME_AMT','SPECIAL_CONSIDERATIONS'
    
What variable(s) are neither targets nor features, and should be removed from the input data?
- The variables that were neither targets nor features and were removed from the input data are the non-beneficial ID columns; "EIN" and "NAME"

#### Compiling, Training, and Evaluating the Model

How many neurons, layers, and activation functions did you select for your neural network model, and why?
- In the original model, prior to optimization, I selected 2 hidden layers with 80 and 30 neurons respectively. Both hidden layers used the ReLU activation function and the output layer used the sigmoid activation function because they matched the complexity of the input data.  

Were you able to achieve the target model performance?
- I was unable to reach the target model performance. The closest I got to the target (75%) was 72.7% accuracy with my original model. 

What steps did you take to try and increase model performance?
- In attempts to optimize my models performance, I added additional neurons to hidden layers, added new hidden layers, changed the optimization function on the hidden layers.

*Below are the results of the original model and all 3 optimization attempts made.*

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

Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.




        Caroline O'Connell
        February 21st, 2021
