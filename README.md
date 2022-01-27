
<p align="center">
    <img src="https://github.com/CharlesDeLabra/Boston-House-Price-Prediction/blob/main/image/boston.jpg?raw=true" alt="Logo" width=72 height=72>
  <h3 align="center">Boston House Price Prediction</h3>
  <p align="center">
    This project uses regression model for predicting prices of house in Boston, based on the features of the houses portrayed on the dataset
    <br>
  </p>
</p>

## Table of contents

- [Context](#context)
- [Problem Statement](#problem-statement)
- [Code](#code)
- [Status](#status)
- [Data Information](#data-information)
- [Analysis](#analysis)
- [Conclusions](#conclusions)
- [Recomendations](#recomendations)

## Context

In Bigger cities there is a tendency of house prices going up and because of this, there is a huge necessity of knowing the prices of houses deoending on aspects such as Neighbourhood, Distance to hubs, Age of house, etc. Boston as a big city have also this problem so there is a lot of data about houses and a crecent necessity for an accurate precision tool.

## Problem Statement

The problem on hand is to predict the housing prices of a town or a suburb based on the features of the locality provided to us. In the process, we need to identify the most important features in the dataset. We need to employ techniques of data preprocessing and build a linear regression model that predicts the prices for us.

## Code

The program was written on Jupyter Notebooks in Python Language. You can access to the code [here](https://github.com/CharlesDeLabra/Boston-House-Price-Prediction/blob/main/Learners_Notebook_Boston_house_price.ipynb)

## Status

The code is finished and have been evaluated, the goal was completed since it were develpo different model in order to predict prices of Boston Houses and they were good enough to trust their predictions

## Data Information

Each record in the database describes a Boston suburb or town. The data was drawn from the Boston Standard Metropolitan Statistical Area (SMSA) in 1970. Detailed attribute information can be found below-

Attribute Information (in order):
- **CRIM:**     per capita crime rate by town
- **ZN:**       proportion of residential land zoned for lots over 25,000 sq.ft.
- **INDUS:**    proportion of non-retail business acres per town
- **CHAS:**     Charles River dummy variable (= 1 if tract bounds river; 0 otherwise)
- **NOX:**      nitric oxides concentration (parts per 10 million)
- **RM:**       average number of rooms per dwelling
- **AGE:**     proportion of owner-occupied units built before 1940
- **DIS:**      weighted distances to five Boston employment centers
- **RAD:**      index of accessibility to radial highways
- **TAX:**      full-value property-tax rate per 10,000 dollars
- **PTRATIO:**  pupil-teacher ratio by town
- **LSTAT:**    %lower status of the population
- **MEDV:**     Median value of owner-occupied homes in 1000 dollars
## Analysis

First it was needed to import the data from the CSV. The dataset look like this:
<br>
<p align="center">
    <img src="https://github.com/CharlesDeLabra/Boston-House-Price-Prediction/blob/main/image/data1.png?raw=true" alt="Data" width=1000 height=500> 
</p>
<br>

After that it was check for multicolinearity and correlation between variables. Then it was decided to drop the TAX column in order to remove the multicolinearity and then a linear regression was trained on the model. The summary of the model was printed and is the next one:
<br>
<p align="center">
    <img src="https://github.com/CharlesDeLabra/Boston-House-Price-Prediction/blob/main/image/data2.png?raw=true" alt="Data" width=1000 height=500> 
</p>
<br>
After that it were removed the variables that did not have a significance of more than 0.05 and then it was printed again the summary of the model:
<br>
<p align="center">
    <img src="https://github.com/CharlesDeLabra/Boston-House-Price-Prediction/blob/main/image/data3.png?raw=true" alt="Data" width=1000 height=500> 
</p>
<br>
The next step was to check for the linear regression assumptions:
- The means of residuals was very close to 0
- Residuals are homoscedastic.
- Residual do not form a linear pattern
- Residuals are normally distributed

Then it was checked the performance on the train and dataset and the results were the next ones:
- Train set: RMSE:0.19 MAE:0.14 MAPE:4.98
- Test set: RMSE:0.19 MAE:0.15 MAPE:5.25

The model is good on both of the data so it was explored if crossvalidation will help us to obtain better results. And with crossvalidation it was obtained a better model which ended being our final model.
## Conclusions

- The value where all the value are 0 is 4.64
- For every unit it increase the Crime rate the value will be lower in 0.0125 of its price
- Same happens with NOX (-1.05), DIS (-0.007), ¨PTRATIO (-0.004) and LSTAT (-0.029)
- When CHAS variable is 1 the price will go 0.12 up
- Same happens with RM (0.05) and RAD (0.007)

## Recomendations

- Depending on the income it is needed to take certain variable in priority
- CHAS and NOX have the higher weight
- If it is important for you the concentration Nitric Oxid and the Charles River boundaries you will have to pay more if you want to be closer to river and you can have a less expensive home if you are in area which are away from industries or with less concentration.
- The safer a house is the expensive the house is, so if you want to locate a safer town you need to pay more by 0.11
- Room per houses is also a variable that will make the house be expensive so the needs of the family are needed to be taken into considerations.
- When a town have a higher displacement to employment centers the price will be lower so if you want to be close to your work probably it will be much expensive
- If there are students taken into consideration if you want the more teachers than students that will mean to pay more
- And also if it is important the status of population in town it is needed to pay more for a better neighbourhood

