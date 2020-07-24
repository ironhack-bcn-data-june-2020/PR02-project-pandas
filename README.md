![IronHack Logo](https://s3-eu-west-1.amazonaws.com/ih-materials/uploads/upload_d5c5793015fec3be28a63c4fa3dd4d55.png)

# Guided Project: Demonstration of Data Cleaning and Manipulation with Pandas

## Overview

The goal of this project is to combine everything you have learned about data wrangling, cleaning, and manipulation with Pandas so you can see how it all works together. For this project, you will start with this messy data set [Shark Attack](https://www.kaggle.com/teajay/global-shark-attacks/version/1). You will need to import it, use your data wrangling skills to clean it up, prepare it to be analyzed, and then export it as a clean CSV data file.

**You will be working individually for this project**, but we'll be guiding you along the process and helping you as you go. Show us what you've got!

---

## What are we trying to accomplish? 

The question I decided to answer were 3 :
### What are the areas with a high concentration of shark attacks?
### What percentage of the attacks are lethal?
### Has de severity of the attacks decreased with time?

To accomplish this the data must be cleaned up since the database is a pretty messy initial state.

### Steps :

1- Import Database & libraries
2- Consult general database information(size,number of null values, what kind of values does each column contain...)
3- Start cleaning , all columns and rows that doesn't provide useful information to answer our questions
4- Manipulate the data to fix some missing values or wrongfully entered values like typo's or years indicated by 0 when on Date we have some dates of reference.
5- We have to transform and apply some functions to some columns to transform the data from float to integers.
6- We can export our cleaned csv and do some calculations to answer our questions.


## What areas did I struggle with? 

I just couldn't manage to fix an issue where some of the years, already converted to integer, were translated into NaN floats when trying to group by 20 the years.

## What could be improved? 

In general the whole project could have a lot to improve , answering more questions, cleaning better and using more pandas tools.
