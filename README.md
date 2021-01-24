# PyBer_Analysis
## Overview
PyBer is a drive-sharing app. I will do analysis for them to improve access to ride-sharing services and determine affordability for underserved neighbourhoods.
In the new assignment, I will use Pandas to create a summary dataframe for riding-sharing data by city type and
use Matplotlib to create a multiple line graph for the total weekly fares for each city type

## Results

### Summary Table
I use pandas to create a summary below:

![summary](/Resources/summary.png)

Acorrding to the table, urban has the biggest amount of total rides and total drivers, while rural is the least.
However, urban has the least average fare price while rural has the largest.

### Multiple line graph
Next, I transferred the long format to wide by column 'type' and get the time from '2019-01-01':'2019-04-29'. The pivot table looks like below:

![pivot](/Resources/pivot.png)

And, I resample() the data by week 'W' and get the sum of the fares for each week as the below picutre shows:
![resample](/Resources/resample.png)

Using the above resample dataframe, I created the below plot:

![plot](/Resources/PyBer_fare_summary.png)

The plot shows urban has the biggest amount of total fare while rural is the least

## Summary
Three Business Recommendations
 - . People in rural and suburban areas need more drivers, because total drivers is less than total rides
 - In urban, total drivers are larger than total rides. Supply is larger than demand. The drivers amount should be decreased.
 - the fare cost in rural areas is too high. It should be decreased.
 