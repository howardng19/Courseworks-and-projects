# Predicting Maximum Wind Speed And Presence Or Absence Of Rapid Intensification With Atlantic Hurricanes Data

This is my final year project of my master degree in Data Science.

This project explores and investigates a dataset provided by WindRisk-
Tech, LLC., which consists of data of Atlantic hurricanes observed between
1979 and 2015. The aim of this project is to investigate to what
extent the maximum wind speed and the presence or absence of rapid
intensification of storms during their lifetime could be predicted with the
provided data. The objective is achieved by first performing exploratory
data analysis, where the data are cleaned and the structures of the data
are revealed before modelling, and unwanted data are filtered out. Next
the target variables are modelled with regression models and classification
models. Regression models to be implemented are Linear Regression
model, Partial Least Squares Regression model and Random Forest Regression
model. Classification models to be implemented are Logistic
Regression model and Random Forest Classification model.

## Folder and files

./report and presentations/ : All presentation slides and report

./hurricane_data/ : The original data provided in .csv

./hurricane_data_analysis.Rmd : The script for data analysis and modelling written in R language (run in RStudio)

## Overview

### The data

The data was provided by WindRiskTech. According to their website, the data were recorded every two hours, and the original dataset consists of the following data as separate files: 1. Day, 2. Hour, 3. Month, 4. Year, 5. Latitude, 6. Longitude, 7. Pressure, 8. Wind speed, 9. Wind shear, 10. Potential intensity. Duration was added as an extra features.
Only those hurricanes with maximum wind speed >= 50 knots were examined in this project.

### Methodology

An exploratory data analysis is first conducted with the dataset, such as cleaning the data, creating a summary dataframe of the dataset and visualising the relationships between variables. With the summary dataframe and the exploratory data analysis as a guide, the maximum wind speed and the presence or absence of rapid intensification of storms are modelled with varied methods. 

The assumptions and theories of all models implemented were discussed. In particular, Linear Regression model, Partial Least Squares Regression model and Random Forest Regression model were implemented to predict the maximum wind speed, while Logistic Regression model and Random Forest Classification model were used for predicting the absences or presence of rapid intensification.
