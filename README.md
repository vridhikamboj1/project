# project
introduction

In this project, we will develop and evaluate the performance and the predictive power of a model trained and tested on data collected from houses in Boston’s suburbs.
Once we get a good fit, we will use this model to predict the monetary value of a house located at the Boston’s area.
A model like this would be very valuable for a real state agent who could make use of the information provided in a dayly basis.

For the purpose of the project the dataset has been preprocessed as follows:
The essential features for the project are: 
CRIM: This is the per capita crime rate by town
ZN: This is the proportion of residential land zoned for lots larger than 25,000 sq.ft.
INDUS: This is the proportion of non-retail business acres per town.
CHAS: This is the Charles River dummy variable (this is equal to 1 if tract bounds river; 0 otherwise)
NOX: This is the nitric oxides concentration (parts per 10 million)
RM: This is the average number of rooms per dwelling
AGE: This is the proportion of owner-occupied units built prior to 1940
DIS: This is the weighted distances to five Boston employment centers
RAD: This is the index of accessibility to radial highways
TAX: This is the full-value property-tax rate per $10,000
PTRATIO: This is the pupil-teacher ratio by town
B: This is calculated as 1000(Bk — 0.63)², where Bk is the proportion of people of African American descent by town
LSTAT: This is the percentage lower status of the population
MEDV: This is the median value of owner-occupied homes in $1000s
RM: average number of rooms per dwelling
LSTAT: percentage of population considered lower status
PTRATIO: pupil-teacher ratio by town


objective

As our goal is to develop a model that has the capacity of predicting the value of houses, we will split the dataset into features and the target variable. 
And store them in features and prices variables, respectively

The target variable, ‘MEDV’, will be the variable we seek to predict. We will store it in prices.

Data Exploration

the minimum value of the house is 105000
the maximum value of the price is 1024800
the average or the mean value of the price is 454342.9
"""
Feature Observation
 


Exploratory Data Analysis
 
 i can begin the process of exploring the data feature by
keeping these three questions in mind:
i) What does the distribution of each feature look like?
ii) If the variables are categorical
iii) If there are missing values, what should be the best strategy to impute them?
i made scatter plot of  RM AND MEDV,MEDV ANDLSTAT,RM AND PTRATIO
all the varibales were numerical
and there were no missing values in the data set


Developing a Model

For this project, we will calculate the coefficient of determination, R², to quantify the model’s performance.
The coefficient of determination for a model is a useful statistic in regression analysis, as it often describes how “good” that model is at making predictions.
The values for R² range from 0 to 1, which captures the percentage of squared correlation between the predicted and actual values of the target variable.
A model with an R² of 0 is no better than a model that always predicts the mean of the target variable.
Whereas a model with an R² of 1 perfectly predicts the target variable.
Any value between 0 and 1 indicates what percentage of the target variable, using this model, can be explained by the features.

Cross-Validation

K-fold cross-validation is a technique used for making sure that our model is well trained, without using the test set. 
It consist in splitting data into k partitions of equal size. For each partition i, we train the model on the remaining k-1 parameters and evaluate it on partition i.
The final score is the average of the K scores obtained

Algorithm
linear regression
lasso regression
ridge regression

result - ridge regression performed better
