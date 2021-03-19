<img src="https://bit.ly/2VnXWr2" alt="Ironhack Logo" width="100"/>

# PR02-project-pandas

Second project of the Module 1

## Content
- [1. Deletion of empty rows](#1.-deletion.of-empty-rows)
- [2. Column analysis](#2.-column-analysis)
- [3. Final dataframe structure](#3.-final-dataframe-structure)
- [4. Pivots & visualizations](#4.-pivots-&-visualizations)

## Project Description
The goal of this project is to combine everything I have learned about data wrangling, cleaning, and manipulation with Pandas to see how it all works together. For this project, I used the messy data set attacks.csv that can be find in this folder. I imported it, used my data wrangling skills to clean it up, prepared it to be analyzed, and then exported it to sharks.csv which can also be found in this folder. 

## 1. Deletion of empty rows
The first step was to delete empty rows, which reduced the size of my dataframe from 25723 rows to 8703.

## 2. Column analysis
The second step was to analyze every column to analyze which method should be applied to each one and execute it. Below there is a list of all columns grouped by the approach I used to cleanse them.

### Case Number & href
The approach for this column was to delete those observations with case number filled but no info in other fields, in addition to comparing the difference between the 3 columns with case number so it's possible to identify where are the mistakes, consolidate all the correct information in one column and delete the other two.

### Datetime
The objective with the date was to create a time series with datetime format. The approach was to create 3 new columns 'Year', 'Month' and 'Day' based on the available information from original 'Date' and 'Case Number' columns.

For those observation with no month on it, a month number was randomly generated. For those ones with no day on it, the value 1 was assigned automatically.

The original column 'Time' was left as originally except for the empty values, which have been filled.

### Country
The approach for the country was to create a new column called 'Country' with the information of the state to which the location belongs and cross it with a .csv file that was previously downloaded from GitHub and rename the original one as 'Geographic Area'.

This file can be found in this folder as countries.csv and from it I extracted the original country for most of the observations and added 2 new columns: 'ISO code' and 'Continent', with the ISO 2-digit code of each country and its continent.

### Location info (location + area + geographic area)
As mentioned before, the original 'Country' column was renamed as 'Geographic Area' and it was concatenated to the other 2 columns related with location: 'Location' and 'Area'. The concatenation of these 3 columns was named as 'Location info'.

### Main activity & main species
For these 2 columns the approach was to leave the original columns 'Activity' and 'Species' as it was, and from each one of them create a new column with the main categories for each one of them, iterate with the most repeated results and add more info to the syntaxis until it's refined enough. For example: walking, floating, standing and bathing can all be grouped as bathing.

### Type, name, injury & investigator or source
For these columns the only action was to fill the empty values and correct a few obvious typos.

### Sex & age
For the 'Sex' column, in addition to correcting a few mistakes, I iterated through 'Name' column so it returns '>1 person' value in case it finds a number. I've realized that most names with a number in it represent several persons involved in the attack.

For the 'Age' column, first I withdrew the numeric values from it. Then I iterated through those values which remained still empty and returned the average of the numbers found as an integer. For example, if originally it comes with a string '23 & 27', the final result will be an integer 25.

### Fatal (y/n)
For this column, in addition to correcting a few mistakes, I returned 'Y' for those values for which column 'Injury' had the word 'fatal' in it.

### Original order & unnamed columns
Original order was just an index upside down, even with a repeated number in the middle of the dataset, so I decided to remove it since we already have an index that sorted the values just the other way around, not upside down.

The other unnamed columns were also removed because they also didn't add value to our datased.

## 3. Final dataframe structure
In this part I sorted the dataframe, removed some unnecessary columns and exported the data to the clean file sharks.csv that can be found in this folder.

## 4. Pivots & visualizations
Last, I provided some examples of pivot tables and visualizations that can be executed with the clean dataframe.



