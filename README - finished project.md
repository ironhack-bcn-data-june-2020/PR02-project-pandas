![IronHack Logo](https://s3-eu-west-1.amazonaws.com/ih-materials/uploads/upload_d5c5793015fec3be28a63c4fa3dd4d55.png)

# Guided Project: Demonstration of Data Cleaning and Manipulation with Pandas

## Process

**Planning the project:** 
The project was planned with Trello. Before I started the cleaning process, I thought of the questions I wanted to answer, which columns I needed to answer the questions and which data format. 
**Importing:** I imported the data easily. I had to do it twice, because if the middle of the project I discovered OpenRefine and decided to use it. 
**Cleaning:** for every column I wanted to clean, I followed the same procedure: 
* First I used the methods describe() and value_counts() to have a general overview of the data. 
* Then I created a dictionary to see all the items in detail, see if there were obvious patterns to make the cleaing easier. 
* I cleaned the values with either OpenRefine, replace or lambda functions, or a combination of the three. 
* I filled the empty values with 'Unknown' in the case of string columns, and with 0s in the integer columns. I considered using the mean of the column, but I thought it would alter the histogram too much so I didn't use it in the end. 
**Manipulation:** I dropped the columns I wouln't need for my analysis. I also dropped all the rows that had 3 or more empty values and all the duplicates in the beginning. As I analysed the Activity column, I realised some accidents didn't involve sharks, so I removed those rows as well. 
**Exporting:** I exported the data easily into a new csv file. 
 

## Results
The final analysis of the dataset reveals that: 
* The top 3 countries where shark attacks occur most often are the USA, Australia and South Africa.
* Most of the people attacked are men.
* In most of the attacks the species is not reported. When it is reported, the top 3 species of attacking sharks are the white shark, the tiger shark and the bull shark. 
* Only 23% of the attacks are fatal, 71% are not fatal and the rest is unknown. 
* Most of the age values of the victims are unknown. Where we do have data, we see that most people attacked are teens or in their 20s. 
* Regarding the evolution over time, the shark attacks have steadily over the years. However, this is not a reliable insight since it's probably due to the fact that the reporting has become more common. 
* The top 3 activities the victims were doing when they were attacked were swimming (includes floating or standing in the water), surfing and fishing.

## Obstacles encountered
* Due to a lack of time I was not able to research more efficient ways of cleaning some data. I had to do a lot of manual replacing in the Countries, Activities and Species columns. 
* Also due to a lack of time I didn't clean the Dates. It was not necessary for the analysis, but it would have been good to practice regex and datetime. 

## Leassons learned
* Basic data manipulation and cleaning with Pandas
* Basic data visualisation with matplotlib. 
* Clustering and merging with OpenRefine. 

## Next steps
* Write more efficient code with more complex functions, possibly using regex. 
* Clean the dates with regex and set them as datetime data type. 
* Create visualizations with several variables (fatality by species, fatality by country, sex by country, etc.)



