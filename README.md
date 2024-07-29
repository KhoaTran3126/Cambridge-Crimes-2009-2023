<h1>An Analysis of Crimes in Cambridge City: 2009 - 2023</h1>

<h2>Introduction</h2>
The following analysis focuses on crime activities solely in Cambridge City, with the <a href="https://data.cambridgema.gov/Public-Safety/Crime-Reports/xuad-73uj/about_data">raw dataset</a> having been provided by the Cambridge Police Department. Crime activities range from the early 1900s to 2024, comprising over 40 various kinds of crimes in Cambridge City. The information provided by the dataset include the date and time of the committed crime, the affected neighborhood, and other. Being more intrigued by the trends of crime activities and the neighborhoods, this analysis focuses on addressing the following questions:<br></br>

<ol>
  <li>What crimes are popular, rising, and dominating in Cambridge City?</li>
  <li>When are the typial hours which crimes are active?</li>
  <li>What neighborhoods are affected the most by crimes?</li>
  <li>What preventative measures may be taken to control the dominant crimes?</li>
</ol>


<h2>Data Processing</h2>
Although the data ranges from the early 1900s to 2024 for the years which various crimes have occurred, few data points exist prior 2009 (which decreases reliability of data) and the data for 2024 is incomplete (and forming conclusions through incomplete data could be fatal): I limited my focus on the range 2009-2023 for most of my analysis concerning years because of those reasons. The 'Crime Date Time' feature is processed such that only the FIRST date and time for each string are retrieved; some datetime strings span more than one date with multiple times, which analyzing the full extent of the period is cumbersome and may be less informative as all the time strings are relatively similar. <br></br>

Any entries with missing values for 'Crime Date Time' are removed because the feature is of interest. For any entries with missing values for "Location" but all other values are intact, the NA are substituted with "UNKNOWN". This is reasonable because any values for "Location" are only estimates of the true location within a 100-block radius. The values themselves are uncertain, as much as the value of "UNKNOWN".

<h2>Data Analysis</h2>
<h3>The Popular, Rising, Dominating Crimes</h2>

![crime count](https://github.com/KhoaTran3126/Cambridge-Crimes-2009-2023/blob/main/plots/crime_count.png?raw=true)

![trends](https://github.com/KhoaTran3126/Cambridge-Crimes-2009-2023/blob/main/plots/trends.png?raw=true)

![relative changes](https://github.com/KhoaTran3126/Cambridge-Crimes-2009-2023/blob/main/plots/relative_changes.png?raw=true)

![densities](https://github.com/KhoaTran3126/Cambridge-Crimes-2009-2023/blob/main/plots/densities.png?raw=true)

![crime hours](https://github.com/KhoaTran3126/Cambridge-Crimes-2009-2023/blob/main/plots/crime_hours.png?raw=true)

<h3>Crimes in Neighborhoods</h2>

![neighborhood count](https://github.com/KhoaTran3126/Cambridge-Crimes-2009-2023/blob/main/plots/neighborhood_count.png?raw=true)

![neighborhood hours](https://github.com/KhoaTran3126/Cambridge-Crimes-2009-2023/blob/main/plots/neighborhood_hours.png?raw=true)

<h3>Preventaion Strategies</h2>

<h2>Conclusion</h2>
