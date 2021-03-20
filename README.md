**1. Importing and general overview:**

I began by importing the csv file and opening it using Pandas, creating a new dataframe named **attacks**.
The next step was getting a general understanding on what I was dealing with, namely the content of the columns. I soon understood that several columns were redundant or simply not of any statistical importance.

**2. Cleaning the columns and empty rows:**

I used *drop* to get rid of redundant/non-relevant columns and *dropna* (with threshold) to delete any rows that were missing so much data thay they were virtually irrelevant to extract any conclusions. I also used *drop_duplicates* to delete any stray duplicate and proceeded to set one column as the index, following a rough chronological order. 
The chronological order wasn't really the goal, I was aiming to simply give all cases a corresponding numerical value for future reference. The fact that I could also have those results in rough chronological order was a nice bonus, but not the main goal.

Before closing this chapter I replaced all *NaN* values for *Unknown*, mainly for aesthetic reasons.

**3. Extracting some conclusions and exporting the csv:**

I used *groupby*, *sort_values* and *rename* to create a new dataset that would contain only the number of attacks by country. I then used *plot* to chart a basic bar graph showing the top 10 countries by number of attacks. Extracting conclusions wasn't an integral part of this project so I didn't expend much time on it.

My idea was to generate a world map with *Folium* showing the cases by country, but I ran into some issues with the indexing. I learned quite a lot about this library while researching this topic and I'm looking forward to applying it to the next project.

Finally, I exported the clean dataframe into a new csv file.


**4. Conclusions:**

While I admit that I didn't spend as much time on this project as I've have liked to, I learnt a lot about using Pandas and most of the techniques teached in class on a real-life messy dataset. I believe that the challenge was both in cleaning the dataset as it was in finding out what was relevant and what was mere trash, or useless data. I'm looking forward to the next challenge!