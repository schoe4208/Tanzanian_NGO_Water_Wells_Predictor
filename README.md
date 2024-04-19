# SWT Clean Water Foundation Presents: Predictive analysis of water wells in Tanzania
![image](https://www.wateraid.org/us/sites/g/files/jkxoof291/files/styles/social_image/public/VFET66_020.JPG?h=5c05d2df&itok=u1yOpny_)

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
![image](https://github.com/schoe4208/Tanzanian_NGO_Water_Wells_Predictor/blob/main/Pictures/EDA%20Exhibit%201%20-%20Water%20Point%20Sources.png)

EDA Exhibit 2: Water points from the Lindi and Mtwara regions had the highest proportion of "Needs Repair" Wells
![image](https://github.com/schoe4208/Tanzanian_NGO_Water_Wells_Predictor/blob/main/Pictures/EDA%20Exhibit%202%20-%20Water%20Point%20Regions.png)

EDA Exhibit 3: Water points managed by schools had the highest proportion of "Needs Repair" Wells
![image](https://github.com/schoe4208/Tanzanian_NGO_Water_Wells_Predictor/blob/main/Pictures/EDA%20Exhibit%203%20-%20Water%20Point%20Management.png)

## Iterative Model Building
SWT Clean Water Foundation constructed the following models:

1. Dummy Classifier
2. Logistic Regression Model
3. Improved Regularization Model
4. Random Forest Classifier

## Conclusion
The improved regularization model was selected as our final model following SWT Clean Water Foundation's model evaluation process. The following recommendations were derived from the Final Model.

1. Prioritize water points sourced from lakes for repairs
2. Prioritize water points in the Lindi and Mtwara regions
3. Management type is not as big of a priority compared with water source and geographic region. If this feature needs to be considered, look at water points managed by schools.

## For More Information
- Detailed Analysis: [Jupyter Notebook]()
- Presentation Deck: [Presentation Deck]()

## Contributors:
- [Sam Choe](https://github.com/schoe4208)
- [Travis Clark](https://github.com/TravisClark1432)
- [William Howard](https://github.com/WilliamHowardGit)

## Repository Structure
```
|— Data                                                      <- Datasets
    |— Training_Set_Values_X_variables.csv                   <- Raw data
    |— Training_Set_Labels_Y_variable.csv                    <- Raw data
|— Pictures                                                  <- Screenshots
    |— EDA Exhibit 1 - Water Point Sources.png               <- Screenshot
    |— EDA Exhibit 2 - Water Point Regions.png               <- Screenshot
    |— EDA Exhibit 3 - Water Point Management.png            <- Screenshot
|— README.md                                                 <- Overview of the Project
|— .gitignore                                                <- List of files to exclude
|— water_well_predictor.ipynb                                <- Detailed analysis in Jupyter Notebook
|_ presentation.pdf                                          <- PDF version of the project presentation slides
