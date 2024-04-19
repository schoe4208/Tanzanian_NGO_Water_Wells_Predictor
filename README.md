# SWT Clean Water Foundation Presents: Predictive analysis of water wells in Tanzania
![image](https://images.app.goo.gl/Ktx3KHXXHKu1ojo66)

## Project Overview
This project investigated the conditions of water points throughout Tanzania with the EDA process examining features such as construction year, water source, geographic region, and management. In addition, the iterative model building process led to the construction of an improved regularization logistics regression model as the final predictive model.

The predictive analysis and proposed recommendations by SWT Clean Water Foundation aim to provide the Government of Tanzania with actionable steps to influence where wells need to be repaired and how new wells should be built.

## Business Problem
Tanzania, as a developing country, struggles with providing clean water to its population of over 57,000,000. There are many water points already established in the country, but some are in need of repair while others have failed altogether.

The Foundation's Data Science Team has been tasked with formulating a predictive model to identify water points that require repairs in order to help the people of Tanzania have increased access to clean and potable water.

## Data Understanding
For the project, the following datasets from the "Pump it Up: Data Mining the Water Table" Challenge were utilized for the predictive analysis:

- Training_Set_Values_X_variables.csv
- Training_Set_Labels_Y_variable.csv

The former consisted of 40 features that made up the set of information about the water points, while the latter consisted of the target variable. SWT Clean Water Foundation elected to feature engineer the ternary classification (functional, functional needs repair, non functional) into a binary classification (functional vs. needs repair) to simplify the predictive modeling process given limited NGO resources. The EDA process then reduced the features down to construction year, water source, geographic region, and management.

EDA Exhibit 1: Water points sourced from lakes had the highest proportion of "Needs Repair" Wells

EDA Exhibit 2: Water points from the Lindi and Mtwara regions had the highest proportion of "Needs Repair" Wells

EDA Exhibit 3: Water points managed by schools had the highest proportion of "Needs Repair" Wells

###

