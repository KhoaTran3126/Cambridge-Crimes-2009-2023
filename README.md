<h1>An Analysis of Crimes in Cambridge City: 2009 - 2023</h1>

<h2>Introduction</h2>
The following analysis focuses on crime activities solely in Cambridge City, with the <a href="https://data.cambridgema.gov/Public-Safety/Crime-Reports/xuad-73uj/about_data">raw dataset</a> having been provided by the Cambridge Police Department. Crime activities range from the early 1900s to 2024, comprising over 40 various kinds of crimes in Cambridge City. The information provided by the dataset include the date and time of the committed crime, the affected neighborhood, and other. Being more intrigued by the trends of crime activities and the neighborhoods, this analysis focuses on addressing the following questions:<br></br>

<ol>
  <li>What crimes are popular, rising, and dominating in Cambridge City?</li>
  <li>When are the typial hours which the top crimes are active?</li>
  <li>What neighborhoods are affected the most by crimes?</li>
  <li>What preventative measures may be taken to control the dominant crimes?</li>
</ol>


<h2>Data Processing</h2>
Although the data ranges from the early 1900s to 2024 for the years which various crimes have occurred, few data points exist prior 2009 (which decreases reliability of data) and the data for 2024 is incomplete (and forming conclusions through incomplete data could be fatal): I limited my focus on the range 2009-2023 for most of my analysis concerning years because of those reasons. The 'Crime Date Time' feature is processed such that only the FIRST date and time for each string are retrieved; some datetime strings span more than one date with multiple times, which analyzing the full extent of the period is cumbersome and may be less informative as all the time strings are relatively similar. <br></br>

Any entries with missing values for 'Crime Date Time' are removed because the feature is of interest. For any entries with missing values for "Location" but all other values are intact, the NA are substituted with "UNKNOWN". This is reasonable because any values for "Location" are only estimates of the true location within a 100-block radius. The values themselves are uncertain, as much as the value of "UNKNOWN".

<h2>Data Analysis</h2>
<h3>The Popular, Rising, Dominating Crimes</h2>

The top most reported crimes in Cambridge city commprise Hit and Run, Larceny acts, and Forgery. Of these top crimes, Larceny of Bicycle displays the most drastic trend from 2009 to 2023; other trends for other activities remain relatively stable, increasing slightly, or decreasing slightly.  

![trends](https://github.com/KhoaTran3126/Cambridge-Crimes-2009-2023/blob/main/plots/crime_count.png?raw=true)

![trends](https://github.com/KhoaTran3126/Cambridge-Crimes-2009-2023/blob/main/plots/trends.png?raw=true)

To further inspect the change in crime activities, another metric is introduced: relative change. Larceny of Bicycle experienced doubled activity in 2023 as compared to 2009, followed by Shoplifting with a little greater than a 50% increase in activity. Surprisingly, Hit and Run activity has increased by a much lesser perentage than either shoplifting or bicycle theft despite being the MOST reported crime. 

![relative changes](https://github.com/KhoaTran3126/Cambridge-Crimes-2009-2023/blob/main/plots/relative_changes.png?raw=true)

The three crimes contributed less than 25% of all crime activities from 2009 to 2022, but contributed slightly to more than 25% of ALL crime activities during 2023. It is also worth noting that the contribution of Hit and Run has remained relatively stable overall with very minor changes: it is Larceny of Bicle and Shoplifiting which are increasing in their overall contribution from 2009 to 2023, so much, they have pushed their cumulative contribution altogether with Hit and Run past 25%. 

![densities](https://github.com/KhoaTran3126/Cambridge-Crimes-2009-2023/blob/main/plots/densities.png?raw=true)

Most crimes occur around 3:00PM, but this is not guaranteed: the time distribution for all the crimes have relatively large spreads around other earlier and later time ranges as well. 

![crime hours](https://github.com/KhoaTran3126/Cambridge-Crimes-2009-2023/blob/main/plots/crime_hours.png?raw=true)

<h3>Crimes in Neighborhoods</h2>
Amongst many neighborhoods in Cambridge City, Cambridgeport and East Cambridge neighborhoods are notably more affected by crime activities as compared to other neighborhoods. But similarly to each other, the time which crime activities are most dominant - including Larceny of Bicycle, Shoplifting, Hit and Run - occur around 3:00 PM with slight variations. It must also be noted that there is a relatively large spread in activity hours around earlier and later time ranges as well.

![neighborhood count](https://github.com/KhoaTran3126/Cambridge-Crimes-2009-2023/blob/main/plots/neighborhood_count.png?raw=true)

![neighborhood hours](https://github.com/KhoaTran3126/Cambridge-Crimes-2009-2023/blob/main/plots/neighborhood_hours.png?raw=true)

<h2>Prevention Strategies</h2>
There is a need for focusing on reducing bicyle theft and shoplifting in all neighborhoods, but more emphasis should be placed on Cambridgeport and East Cambridge. the preferred regulation time should be around 3PM, but extending also to earlier and later time ranges. There also requires regulation against Hit and Run, but perhaps less extensively than the other two, having seen how Hit and Run has increased with a lesser magnitude.

<h2>Conclusion</h2>
Of the numerous crimes analyzed, three stands out prominently: Larceny of Bicycle (Bicycle theft), Shoplifting, Hit and Run. Although Hit and Run is the most reported out of more than 40 crimes, increases in the activity of Hit and Run pales in comparison with the increased activity observed in Larceny of Bicycle and Shoplifting. The most affected neighborhoods are Cambridgeport and East Cambridge. All crimes occur most prevalently around the time range of 3PM. Although there are more than three crimes requiring proper regulation, this analysis focuses only on the top, increasing crimes: there is a need to better regulate incidents of bicycle theft and shoplifting if it is the overall wish to bring their occurrences down to stability, away from their increasing trends. Hit and Run also requires regulation, but with lesser effort as compared to the other two crimes which have increased much more drastically in their occurrences from 2009 to 2023. 
