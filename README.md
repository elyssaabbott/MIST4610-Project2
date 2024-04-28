
# MIST 4610 Project 2

20244 Group 3

1. Elyssa Abbott @elyssaabbott
2. Nicolle Serafin @nikkiserafin
3. Shubhangi Khanna @shubbykhanna
4. Jay Dumon @JayDumon
5. Ryan Cullen @javaprogrammer2023
6. Shriya Tummalapalli @shriyatummalapalli

## Data Description

 The data we are working with is the NYPD arrest data from 2023. The data was obtained from data.gov (https://catalog.data.gov/dataset) and the specific dataset can be found here (https://catalog.data.gov/dataset/nypd-arrest-data-year-to-date). We decided to go to the publisher’s website and collect more data as our dataset was not complex enough for our analysis, Therefore, our dataset consists of 571,711 rows of data and 24 columns describing the number of arrests and other information related to these arrests from January 1st, 2021, to December 31st, 2023. Every time an arrest is made, it is added to this dataset so that it can be reviewed by the Office of Management Analysis and Planning every quarter. The data recorded includes information about the date of the arrest, a description of the reasoning for arrest, where the arrest was made, and the perpetrator’s race, sex, and age group.

The arrest key is the dataset’s primary key. Every time an arrest is recorded, it is given its own unique identifying arrest key. The next column is the arrest date which is in the date-month-year format. PD CD is the next column, and after researching, we believe this is the police department communications division. This column has an int data type. There are also police descriptions and offense descriptions in the data. Police descriptions are a little more specific than offense descriptions as offense descriptions is the category that police descriptions fall under. Both of these columns have varchar data types. Other related columns are the KY CD, law code, and law category CD. The KY CD column most likely refers to the code entered for the PD description, and the law code and law category CD most likely refer to the offense description. KY CD has an int data type, law code has a varchar data type, and law category CD has a varchar data type. The next columns are arrest borough, arrest precinct, and jurisdiction code. Essentially, these columns are describing which of the five New York boroughs the arrest was made, in what precinct, and with what jurisdiction code. They have a varchar, int, and int data type respectively. The following three columns are characteristics of the person that was arrested including the age group, sex, and race, and all three columns have varchar data types. The next columns describe the exact location where the arrest was made. X coordination, y coordination, latitude, and longitude. X and y coordinates are int data types, while latitude and longitude are decimal data types. Longitude Latitude is the next column with a varchar data type that combines the longitude and latitude points in the previous columns. Following this column are the Zip Codes, Community Districts, Borough Boundaries, City Council Districts, and Police Precincts. The column Zip Codes has a varchar data type while the remaining columns have int data types and also describe the location of the arrest.

The dataset is appropriately and sufficiently complex because it includes multiple years of relevant data. With this data we are able to forecast future arrest trends and determine which age groups are the most prevalent in arrests. When it comes to variance in the data, our dataset has a low variance because the data does not deviate much from the mean. This demonstrates a more uniform and consistent pattern making it easier to draw conclusions about arrests and identify patterns in the data.


## Questions and Importance

What type of crime is most prevalent for each age group in New York?

Importance: Based on the data evaluation this question is relevant because it can help law-enforcement officers identify trends and use this to prevent future crimes by staying equipped. By analyzing this data through age group officials can address root causes and provide adequate solutions to these problems. To depict this visually we chose to create bar charts for different data groups so officials can see what kind of crimes are happening and how they can effectively put a stop to it.


Over the course of 2021 to 2023, what is the trend of arrests for each location based on borough for age group 25-44?

Importance: To enhance our data analysis, we narrowed our focus to the age group with the highest number of arrests, which was 25-44. We then delved deeper by examining trends in crime rates within this age group across different boroughs. This analysis is significant because it could allow us to explore potential correlations between crime rates and various factors such as population demographics and economic conditions in the future.

## Manipulations

In order to ensure understanding of our data visualizations, a calculated field was created to translate the codes for the boroughs into the full names of them. This way when looking at the line chart, it can be easily understood which borough is which line. We also filtered by month and used the color feature to distinguish the boroughs, as well. Additionally, the team chose to forecast the data to identify potential trends in the future.   

## Analysis and Results

UNDER 18 OFFENSE DESCRIPTIONS:

For this age group (under 18), the number of offenses committed (across all categories) is the second lowest compared to the rest of the age groups. In addition, the category with the highest offenses is “robbery”. This differs from the rest of the age groups, where the other age groups have “assault” as the category with the leading number of offenses.

18-24 OFFENSE DESCRIPTIONS:

The overall volume of arrests for this age group (18-24) is much higher than for the under 18 age group. Both age brackets share the same top four offense categories. However, for the 18-24 age group, we see assault and felony assault leading the way, setting a trend for the rest of the age groups.

25-44 OFFENSE DESCRIPTIONS: 

Similar to the other age groups, the highest categories are assault, both misdemeanor and felony. However, there is a significant difference in the counts of multiple of the top offense description categories by the thousands; the top categories have the highest number of arrests by far, with over 53,000 arrests for misdemeanor assault alone, compared to the highest category from all other age groups being less than 18,000.

45-64 OFFENSE DESCRIPTIONS:

Similar to the two age brackets, assault is the leading category for offenses. However, the number of offenses committed in this category decreased by about 66%. To clarify, in the 25-44 age bracket, there were a little over 53,000 offenses. However, in the next age bracket (45-55), there were around 17,000 offenses. This trend seems to continue for other offense categories. 

65+ OFFENSE DESCRIPTIONS:

Overall, this age bracket (65+) had the lowest amount of offenses per category, compared to the remaining age brackets. Similar to the previous age groups, assault was the leading offense category. Some of the age brackets had the same top four offense categories, and this last age group seems to continue that trend.

FORECAST DESCRIPTION:

In this graph, we captured the number of arrests per borough for ages 25-44 from January 2021 to December 2023, with a forecast for January 2024 to June 2024. All 5 boroughs (Bronx, Brooklyn, Manhattan, Queens, Staten Island) have some fluctuation with the number of arrests per month, which is showcased in the graph. Staten Island starkly has the lowest number of arrests compared to the other boroughs. However, the forecast seems to increase the number of arrests, which seems to be true for all boroughs. The Bronx seems to have the highest arrests, followed by Brooklyn, Manhattan, Queens, and then Staten Island. It’s interesting to see the forecast also fluctuating with the arrest count.


##  Tableau Packaged Workbook

Link: https://outlookuga-my.sharepoint.com/:u:/g/personal/eaa26824_uga_edu/ERIgBZkBZVlNqp5wqgMO0VoBaWsGSigX0pP_vhqN8m9gcQ?e=1NbP5k
