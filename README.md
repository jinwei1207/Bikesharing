# Tableau Bikesharing Analysis

## Project Overview
The purpose of this project is to create a visual business proposal using [Tableau Public](https://public.tableau.com/en-us/s/). Data on Citi bike ridership in New York City is analyzed to determine the business prospects of creating a similar business in Des Moines, Iowa. Pandas DataFrames and Tableau Calculated Fields are used to transform the datatypes and format of some columns.



### Correcting the Gender Column 
The column "Gender" was originally formatted as 0, 1, and 2 to identify genders (Unknown, Male, and Female). To have this column correctly print with letters instead of numbers, the datatype of the column is changed to string and the following code was used to create a calculated field: 
```tableau
if [Gender] = '0' then 'UNKNOWN'
ELSEIF [Gender] = '1' then 'MALE'
ELSEIF [Gender] = '2' then 'FEMALE' END
```

## Results 
[Click here to view the completed Tableau business proposal.](https://public.tableau.com/app/profile/wei.jin4205/viz/NYCsotry/NYCStory?publish=yes)

![image](https://user-images.githubusercontent.com/104603177/184060611-5bb55dc5-9abf-4ebd-b39c-eb0a7004b209.png)

81% of the users were subscribers. 65% of the users were confirmed males and 25% were confirmed females.
![image](https://user-images.githubusercontent.com/104603177/184060039-9438e3bf-c9f6-4cd8-9af3-b9612470be7b.png)


Total user checkout times are then shown, which is then followed by the same graph filtered by gender and hour. This line graph showcased the large disparity in Male and Female ridership.
![image](https://user-images.githubusercontent.com/104603177/184060186-ce01639a-e6fe-4456-a66b-c32160b2f2a5.png)

Total trips by weekday are visualized as a heatmap. The majority of Monday-Friday each hour. When filtering this heatmap by Gender, it is again found that Male ridership far outpaces Female ridership. However, the peak riding hours across all genders are similar.
![image](https://user-images.githubusercontent.com/104603177/184060275-99787b64-25b0-455d-96c7-a10fe5586f04.png)


Finally, user trips by gender is visualized. This chart illustrates that users are much more likely to be subscribers, rather than ordinary customers.


## Summary  
The data shows high activity of the bike sharing service in New York during the month of August 2019.
The far majority of the rides were in the very busy Manhattan Island, taken by male users during morning and evening rush hours. This implies that Citi Bike services are used as an alternative to public transportation by commuting workers.

### Additional Suggestions
In addition to the analysis presented in this Tableau Story, two more visualizations are suggested for future investigation:
1. The top starting and stopping location by gender. This visualization will determine whether there is a gender disparity between the locations were rides begin and end.
2. Usertype percentage by gender should be investigated. If there is a difference between gender and usertype (subscriber vs customer), there could be a more targeted advertisement campagin if this new business is established.

