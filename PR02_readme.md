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

The questions I want to answer with this analysis are:
- have there been more shark attacks in Australia or in the USA?
- have they been made to surfers or swimmers?
- in which period of the year are there more sharks attacks and in which country?
- are the victims of fatal attacks more women or men?

The columns to use for the analysis are: 'Case Number', 'Date', 'Year', 'Type', 'Country', 'Area', 'Activity', 'Sex', 'Injury', 'Fatal (Y/N)'



## Workflow


1. Creation and exploration of the DataFrame: column analysis and nulls count
2. Exploration of the original Dataset (size: 25723 x 24)
3. Modification of the name of the columns (elimination of white spaces) and elimination of the rows with all missing values size: (size: 8703 x 24)
4. Export the results in a new file 'attacks-reduced.csv' for consulting it, if necessary

**Let's get started with the Analysis!**
1. Creation of a new DataFrame with a reduced number of columns (size: 8703 x 10)
2. Reduce number of rows, keeping only the rows with at least 6 non NaN values (size: 6302 x 10)
3. Detection of the duplicate records based on the column 'Case Number'
4.
5.


## Organization

The repositoy contains these files and folders:

- input folder: contains the original dataset and the reduced one
- output folder: contain the results of the Analysis
- working files: data-wrangling.ipynb (jupyter notebook)
- .gitignore
- PR02_readme.md
## Links

[Repository](https://github.com/)  
[Slides](https://drive.google.com/drive/folders/1-3pDeIjQp9MNMQCVvtrebRMLDuLVeCKz)  
[Trello](https://trello.com/b/cVNiEA6v/project-1-mastermind)  
