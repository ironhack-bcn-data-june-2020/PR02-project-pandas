
# Sharks Attacks

## Overview

The goal of this project was to combine everything I have learned about data wrangling, cleaning, and manipulation with Pandas. 

## Steps followed: 

- Imported the file 
- Used my data wrangling skills to clean it up and prepared it to be analyzed
- Exported it as a clean CSV data file : sharks_clean

## Data Cleanning: 

1. I checked "info" and "shape" to see what kind of dataframe I was working with.  
2. I did a "general cleanning":

* Deleted all the rows with only NaNs 
* Deleted all the duplicate rows 
* Deleted the rows that don't have content in at least 3 columns 

3. I use display.max rows and display. max columns to visualise the whole content. 

4. Columns I cleaned:
- Species:
- Age 
- Type
- Case Number
- Activity 
- Sex
- Fatal 
- Country
- Year

5. Methods used:
- dropna
- drop_duplicates
- fillna
- sort_values
- value_counts()
- nlargest()
- str.replace
- regex
- to_datetime
- apply()
- x.strip()
- x.title()
- lambda
- isin()
- plot
- pivot_table

## Lessons learned: 

- I should have spent more time analysing the data before starting to clean it (Ex: Case Number easier to clean than Date)
- I should have used Regex from the beginning
- I should have used less "replace" (next time I should use find)
- I should practice regex more
- I should have used group by and more pivot tables, melt
- Next time I will try to use open refine (for the clusters) 
