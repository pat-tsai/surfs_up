# Surfs up
climate analysis using python and sqlite

## Overview of analysis: 
The purpose of this analysis was to connect and retrieve datasets from SQLite databases to ultimately calculate temperature summary statistics. These results are used to analyze how well a surf and ice cream shop business would thrive based on monthly weather conditions.

# Results:
![ScreenShots](/june_december_summary.png)

Shown above are the summary statistics for June (left) and December (right). 
- 1. Conventionally, June is typically one of the hottest months, whereas December is typically among the coldest. The summary statistics summary follows this same trend, with June having a mean temperature of about 75 degrees, and December having around 71 degrees. These temperature would be nice to enjoy ice cream/go surfing.
- 2. June temperatures have a standard deviation of 3.26, whereas December is 3.75. This reveals larger fluctuations in December temperatures, reflected by the larger range from min to max December temperatures (56 minimum, 83 maximum)
- 3. There are 1,700 non-null datapoints for June, but there are only 1,517 for December (missing half a year of data). This is likely due to the timing of gathering data, and since December is in the 2nd half of the year the data may not have been available when this dataset was made. Including the missing 183 days would likely alter the December statistics, possibly lowering the standard deviation if the temperatures following past year's trends.  

# Summary
Based on the above analysis, additional queries that could be performed for further analysis includes:
- 1. Adding additional filters within each month to split each month's data into 4 more groups (ie. calculating summary statistics for weeks 1-4 of June and December). This would allow us to more closely compare data and how the temperatures vary between each week for each month. 
- 2. Filtering and calculating/plotting monthly temperatures grouped by each year to better display fluctuations within each month. Since our current summary statistics are calculated by combining all data within the database (2010-2017), we could get a better sense of temperature fluctuations within each year by calculating seperate tables of summary statistics for both June and December in each year from 2010 to 2017, resulting in 14 new summary tables total. Furthermore, we could plot these results on a line graph to see how the trends vary monthly/annually. 

In conclusion, based on the temperature analysis it seems like Oahu would be a prime spot to open a surf and ice cream shop.
