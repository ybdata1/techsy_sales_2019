You're back!

Okay, so as noticed when trying to manipulate the data, we have some non-conforming values in our raw data. These 
values are the result of concatenating entire order sheets together in a monthly sheet with the header included,
and each month had mutiple "sheets" stitched together this way. This header was preventing us from assigning 
the correct data types in pandas to improve performance. 

My first instinct was to manually go and remove each instance of the header. After doing this 6-7 times, I 
realized I was only 1/10 of the way through the first month of data, with 11 more months to go. Clearly,
this method was inefficient. After some thinking, I decided to go with the following method:

1 - Use Crtl+F to find all instances of the header
2 - Select all instances (except for the first row)
3 - Delete these rows
4 - Repeat 11 times

Now, technically I could have combined all the sheets into one workbook and done it in one sweep, but I already
had all 12 month files open in excel in preparation for method #1. I figured it would take me just as long to
do it this way. The header appeared between 19-37 times per sheet, so doing this process in 12 steps rather 
than 200+ counted as a win in my book.

The resulting files were saved with a "_formatted.csv". 12 in total. I copied these files over to folder 2 to
continue my data cleaning with python/pandas.

You can return to folder 2 for rest of the cleaning process.