I opened my first python script after taking a quick review of the data. I imported each csv file as its own
dataframe, making 12 total (with all blank rows dropped). I quickly ran into a problem:

Our dataframe columns were not acting correctly. I ran into errors that had shouldn't have been there. After
reviewing my code a few times, I determined I didn't make any coding errors. My logic was fine. So what was
going wrong?

Turns out these dataframes held some values that were incongruous with the rest. These string values 
prevented us from assigning data types, which would both improve performance and let us manipulate
the data more easily/cleanly. If you want to find out how I fixed this, go to ("1 - Raw Data/README_2.txt")

============================================================================================================

You're back!

The rest of the data process was fairly standard. Occasionally, I'd forget a method and have to look it up,
but these setbacks only last between 3-5 minutes. I spent a good amount of time testing the script as well
to make sure it ran correctly. For more details, I invite you to read the script file:

("2 - Python Data Cleaning/Script1 - Techsy Sales Data Cleaning.ipynb")

I made sure to put notes at the top of each cell to make it easy to follow along. Once this was done, I had 2
result files: "products.csv" and "Sales_2019_Cleaned.csv"

I copied these files over to folder 3 to import them into Power BI for data modeling/visualization.