# Surfs_up

## Overview of Surfs Up Analysis:
The purpose of this analysis is to review a dataset pertaining to weather conditions that has been stored in a SQLite database to provide information that will convince an investor that opening up a Surf n' Shake shop in Oahu, Hawaii is a good business idea. The idea is that the shop will sell surf boards and ice cream throughout the year, but the investor is hesitant because he invested in a similar business that failed due to the weather conditions. In order to get this investor on board, we need to provide statistical analysis specifically on the weather conditions in Oahu that will convince him that this will be a successful business venture.

In order to explore the data in the SQLite database, we used SQLAlchemy to connect and generate queries to pull the necessary information needed for our analysis. Throughout this module, we used Jupiter notebook to import dependencies and create the commands to pull the data from the SQLite database. 

# Results

## June and December Temperature Findings
Using Python, Pandas , and SQLAlchemy, the date column of the Measurements table was filtered in the hawaii.sqlite database to retrieve all the temperatures for the months of June and December. Those temperatures were converted to a list, a DataFrame was created from those lists, and then summary statistics were generated for each dataset.

June temperature statistics showed the following:

![image](https://user-images.githubusercontent.com/92283185/146712725-d62a0941-4b1d-4915-a0a9-41a062fb866e.png)

December temperature statistics showed the following:

![image](https://user-images.githubusercontent.com/92283185/146712780-814c4d69-e41d-4e92-aec9-6deeeba8afd8.png)



Comparing the temperatures for the two months, we can see the following:

- There were 12% more temperature points for June than there were for December.
- The average temperature for December was 71 degrees, which is nearly four degrees cooler than June's average temperature of 74.9 degrees.
- The maximum temperature for June was 85 degrees, which is only two degrees warmer than December's maximum temperature of 83 degrees

## Summary

To summarize this analysis We also looked at the number of weather stations that were actively collecting precipitation data and we tried to focus on one station that had the most observations recorded. In total, there were (9) stations with USC00519281 showing the highest amount of observations at 2,772 entries. We used the information from this station to review the temperature for the same time period. The results showed that the average temperature throughout the year was 72°F with a low of 54°F and a high of 85°F. For that I wrote the follwoing query and also generated the plot to have better understanding :
- Query 
![image](https://user-images.githubusercontent.com/92283185/146713535-315cedce-b1f4-4216-9adc-567f4d7a8fe8.png)

- Visual presentation :

![image](https://user-images.githubusercontent.com/92283185/146713586-17fe3db2-4406-46b7-b6b8-676cda8565a5.png)


In order to fully understand the weather trend, I ran an additonal query on:

- Precipitation to observe quantity and frequency during June and December, and determine whether precipitation plays a factor despite the warm temperatures that are experienced during this time.

 
![image](https://user-images.githubusercontent.com/92283185/146712950-75a93c91-f7c3-4b84-b68a-4fac136a26bb.png)
![image](https://user-images.githubusercontent.com/92283185/146712985-587a036d-445f-40aa-b571-fd837208e3ea.png)

From the above table we can see the following:
  - There were 12% more precipitation points for June than there were for December.
  - The average precipitation amount for December was 0.22 inches, which is 0.08 inches more than June's average precipitation of 0.14 inches.
  - The maximum precipitation amount for June was 4.43 inches, which is close to 2 inches less than December's maximum precipitation amount of 6.42 inches.

Looking at the precipitation and the temperature proves that investing in Surf n' Shake is a good business venture and that Oahu, Hawaii is the ideal location.

