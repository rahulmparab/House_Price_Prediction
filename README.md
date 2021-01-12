# Project 2 - Ames Housing Data and Kaggle Challenge : submission by Rahul Parab

**Notes**
In this project, I created a Linear Regression model using Ames Housing Dataset. The main obective of this project is to predict the price of a house at sale. 
 
## The Modeling Process

1. There are 2 data sets train and test. The training data set has all the parameters along with the house price at sale, where are test data has only the paramters. The main aim of this project is to build and train a linear regression model on the trainig data set and then predict the house sale price for the test data. 
2. Here are the steps followed in the model building process : 
    - EDA
        - Addressing NULL columns
        - Generate a heat map to understand correleation between input variables and Predicted value.
        - Sale price : distribution
        - Find and Remove outliers     
    - Build a null model using all numeric features - this will act as a baseline for model tuning.
    - Analyze non-numeric parametes : categorical variables are dummified 
    - Feature selection : 
        - In an iterative mode, 
            - select features one at a time 
            - add this to a feature list 
            - run the linear regression model and store the score in a list
        - once all features are utilized, 
            - compare the scores and pick the model with best score 
            - this is the list of best features to be included in the final model 
    - The provided training data is further split into train , test (80,20)  
        - Model accurancy for train data is 87.98 and for test data is 87.92
  
