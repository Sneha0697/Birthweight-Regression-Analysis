# Birthweight-Regression-Analysis
Determine the best regression model for predicting the behavior of explanatory variables such as parent age, education, alcohol consumption, and so on, in relation to the dependent variable, neonate weight.
## Introduction
The purpose of regression analysis is to determine the impact of a combination of explanatory variables on the dependent variable. Predicting the price of a house based on current market conditions, geography, demand, and supply, for example. The R-value indicates the extent to which the explanatory variables influence the dependent variable. In a given circumstance, an analyst's job is to anticipate which experimental variables will have the strongest influence on the determining variable and to do so with the least amount of error. As a result, we employ trial and error to select the final set of variables that influence the determining factor to the maximum extent possible. In addition, multiple regression models are used to assess and improve prediction accuracy. In this project, we will use this approach to investigate how various parental characteristics influence the weight of a newborn.
## Types of Regression Models
Many regression models are available to aid in the prediction. Linear Regression, Logistic Regression, Lasso Regression, Ridge Regression, Polynomial Regression, and others are examples. In this work, we used four different types of regression models. They are explained further below.
### OLS regression Model
OLS abbreviated as Ordinary Least squares s used to determine the simple linear regression of a collection of data. The equation below is used to denote the linear regression model.</br>
y = mx + c + e </br>
where m = slope of the line </br>
      c = intercept </br>
      e = error in the model </br>, here the predictor error is defined as the difference between the observed and predicted values.
The error in the OLS model is simply squared, i.e., e2, then added to yield the overall error. This is done to lessen the overall error. Vertical lines in the graph below represent the error (e).
A standard curve for a linear regression model

 I have classified all of the variables in the project as continuous or countable. The linear regression model has then applied to the group of continuous variables. After a few regressions with various combinations of those variables, the final set of variables with the highest R- value has been chosen to utilize in further regression models.
### Lasso Regression Model
Least Absolute Shrinkage and Selection Operator is abbreviated as Lasso. In order to minimize prediction error, this model employs the shrinking strategy. It imposes a limit on the model parameters, causing some variables' regression co-efficient to dwindle towards zero. Shrinkage can alternatively be defined as the data variables shrinking towards their central points, such as the mean.
The Lasso Regression technique is represented by the following equation:
N^{-1}Σ^{N}_{i=1}f(x_{i}, y_{I}, α, β)
### ARD Regression Model
The Bayesian Inference Method underpins the Automatic Relevance Determination (ARD) Model. The ARDRegression considers the model weights to be Gaussian and iteratively calculates the lambda and alpha parameters. Alpha() is a hyperparameter vector that specifies how far each weight can deviate from zero.
## Conclusion
After dividing the data into trial and test sets and fitting those sets into several regression models, the Lasso Regression Model showed to be the best model for the given data, with higher training and testing scores and the smaller test gap. 
