
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

## Analysis

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

