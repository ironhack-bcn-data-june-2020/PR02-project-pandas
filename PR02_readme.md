<img src="https://bit.ly/2VnXWr2" alt="Ironhack Logo" width="100"/>

# Shark-Attacks
*Veronica Agnolutto*

*Data_Barcelona_july.2o*


## Content
- [Project Description](#project-description)
- [Analysis](#Analysis)
- [Workflow](#workflow)
- [Organization](#organization)
- [Links](#links)


## Project Description

This project consists in analyse a Kaggle data set [Shark Attack](https://www.kaggle.com/teajay/global-shark-attacks) and apply tools and techniques of data cleaning and manipulation with Pandas.


## Analysis


To limit the information that can be found in a dataset, it is better to think about an hypothesis...


## Hypothesis


IN THE LAST EIGHT YEARS THE NUMBER OF SHARK ATTACKS HAS BEEN CONSTANT ALL OVER THE WORLD

The columns used for the analysis are: 'Case Number', 'Date', 'Year', 'Country', 'Area', 'Activity', 'Sex', 'Injury', 'Fatal (Y/N)'

All data before 1600 AD are not considered.


## Workflow


**Cleaning**
1. Creation and exploration of the DataSet
2. First reduction of the number of rows (based on the initial hypothesis of valid years) and columns (based on nulls values)
3. Cleaning text and modification of the data types
4. Replacing missing values
5. Export the results in a new file 'attacks-reduced.csv' for consulting it, if necessary


**Let's get started with the Analysis!**
1. Creation of a new DataFrame with only the columns for analysis
2. Drop the duplicate records
3. Verify my hypothesis
4. Export the results


## Organization

The repository contains these files and folders:

- input folder: contains the original dataset and the reduced one
- output folder: contains the results of the Analysis
- working file: data-wrangling.ipynb (jupyter notebook)
- PR02_readme.md
- .gitignore


## Links

[Repository](https://github.com/)   
[Trello](https://trello.com/b/AajLeNZC/pr02-sharks-attacks)  
