# PyBer Analysis
*Matplotlib Analysis for PyBer Ride-Share company*

## Project Overview 
### Purpose

The purpose of this analysis is to perform data analysis for Ride-Share company *PyBer* and to tell compelling story with data visualization. This analysis showcases the relationship between the type of the city -- urban, suburban and rural -- and their correlation between rides, drivers and fares, and congregates data from January to early May of 2019 and focuses on the following: 

-	The total number of rides for each city type. 
-	The total number of drivers for each city type.
-	The sum of the fares for each city type.
-	The average fare per ride for each city type.
-	The average fare per driver for each city type.
-	The total fares for each week by city type. 

### Background
The data is gathered in two different CSV files (the city data and the ride data). In this analysis I am using **Jupyter notebook** and **Pandas Library** to inspect data, merge datasets, perform calculations an create data series and data frames. In addition to this I am using Python’s plotting library **Matplotlib** in order to tell visual story and to present complex findings in more informative and engaging way. Data Visualization allows audience to absorb information quickly and detect patterns, trends, correlations and outliers in more effective way.

### Overview the methods and code
#### Matplotlib
Matplotlib is a Python graphing library and offers wide range of graphs, from line plots to 3D plots and it is widely used amongst data analysts. It also has rich styling options and customizable annotations. Matplotlib has two graphing methods: Pandas **MATLAB** and **The object-oriented method**. MATLAB plotting is used for quick and simple plots that require little coding, while the object-oriented method is used for more complex graphs, including those with multiple plots on the same graph and require more coding (1). 

Besides [official Matplotlib documentation]( https://matplotlib.org/3.2.2/users/index.html), Matplotlib offers many default plot settings that already have integrated many features and require little coding and results in sophisticated graphs. For example, *Stylesheets* offer a number of default styles with the ability to create and package your own styles. One of them is **FiveThiryEight style** and it is typified by bold colors, thick lines, and transparent axes (2). Those styles can save us lots of time and coding.

<p align="center">  
<img src="Graphics/FiveThirtyEight.PNG" width="30%" height="30%">
</p>
<p align="center">  
An example of FiveThirtyEight StyleSheet from Matplotlib default plots.
</p>

#### Exploratory data analysis or EDA
EDA is an important step in data analytics. This critical step **can save roughly 15–50% of time on a project** because it provides a targeted plan for how to clean, sort, and create smaller datasets, that is easier to work with (3). Also, we could describe EDA as in **“A first look at the data”** and it is used **to understand and summarize the content of the dataset**, such as initial look at the columns, datatypes, data quality, data statistics and data relationships (4). Besides checking data in **"non-graphical" way**, it is a good practice **to check data "graphically"**. For example, box and whiskers graph below quickly determine outlier(s), that are harder to determine by "non-graphical" way. **Inspecting data quality** (missing values, possible duplicates, outliers and other anomalies) it is an important step and can have big impact on the data analysis and the story we want to tell. We can decide how to treat those by including them or omitting them from the further data analysis.

<p align="center">  
<img src="Graphics/Outlier.png" width="50%" height="50%">
</p>
<p align="center">  
Determine an outlier(s) with box and whiskers plot.
</p>

## Resources
- Data Source: 
  - [city_data.csv](Resources/city_data.csv)
  - [ride_data.csv](Resources/ride_data.csv)
- Software: 
  - Jupyter Notebook 6.0.3 <img src="Graphics/JupyterNotebookLogo.PNG" width="3%" height="3%">
- Environment: 
  - Python 3.7 <img src="Graphics/PythonLogo.PNG" width="3%" height="3%">
- Dependencies:
  - Matplotlib Library 3.2.1 <img src="Graphics/MatplotlibLogo.PNG" width="6%" height="6%">
  - Pandas Library 1.0.5 <img src="Graphics/PandasLogo.PNG" width="6%" height="6%">

## Results 
From the table *The Summary Data Frame per City Type* we can see the results for each city type – urban, suburban and rural in correlation to the amount of rides, drivers and fares from January to early May of 2019.

<p align="center">     
<img src="Analysis/TheSummaryDataFrame.PNG" width="80%" height="80%">
</p>

**1.	The total number of rides for each city type.** 
  -	The total amount of rides is 2.6-times higher in urban cities than in suburban cities.
  -	The total amount of rides is 13-times higher in urban cities than in rural cities.

**2.	The total number of drivers for each city type.**
  -	The total amount of drivers is almost 5-times higher in urban cities than in suburban cities.
  -	The total amount of drivers is almost 31-times higher in urban cities than in rural cities.

**3.	The sum of the fares for each city type.**
  -	The total amount of fares is 2-times higher in urban cities than in suburban cities. 
  -	The total amount of fares is 9-times higher in urban cities than in rural cities.

**4.	The average fare per ride for each city type.**
  -	The average fare per ride is 1.3-times lower in urban cities than in suburban.
  -	The average fare per ride is 1.4-times lower in urban cities than in rural cities.

**5.	The average fare per driver for each city type.**
  -	The average fare per driver is about 2.4-times lower in urban cities than in suburban cities.
  -	The average fare per driver is about 3.3-times lower in urban cities than in rural cities.

**6.	The total fares for each week by city type.**

  From the multi-line graph *Total Fare by City Type* we can see the results for each city type – urban, suburban and rural in correlation to the total fare amount per week from January to the end of April 2019. 

<p align="center">     
<img src="Analysis/PyBer_fare_summary.png" width="60%" height="60%">
</p>

  -	Urban cities have the highest total fares overall. The amount is ranging from the lowest at about $1,600 per week to the highest at about $2,500 per week. 
  -	Rural cities have the lowest total fares overall. The amount is ranging from the lowest at about $250 per week to the highest at about $500 per week.
  -	Suburban cities fall in between. The total fares amount is ranging from the lowest at about $650 per week to the highest at about $1,450 per week.
  -	All cities have pretty steady flow of total fares from week to week with a matching spike in the third week in February.

## Summary 
The obvious point from the result above is disproportional distribution rides and drivers amongst the city type. Urban cities have much higher number of rides and drivers; however, the average fare per ride and per driver is lower than in suburban and rural cities. 

1. **Rural cities have the lowest amount of the rides and drivers**, yet the ratio ride to driver is the highest (1.6 compare to 0.67 in urban cities). This indicates fewer drivers in rural cities per ride than in the urban cities. Increasing number of drivers could have positive affect on total amount of fares, yet some additional questions need to be answered before making final suggestions.
- Is PyBer profitable in rural cities compare to the suburban and urban cities? Although the sum of total fares is low, it could still be profitable. 
- What is the ride count per capita compare to other types of the cities? Lower population could cause low ride and driver count and lower need for PyBer service. 
- What is the average length of the ride? High amount of the average fare can be affected by lengthy rides that results in higher average fare per ride.
- How frequently do residents of rural cities use public transportation? Some rural cities might require more PyBer services than others, so focus on increasing service could go to those specific cities.

2. There is **a matching peak in third week in February for each city type**. Based on this information I would suggest to research this peak in more detail that can help determine what caused the jump. Therefore, the analsis can be used as a business strategy in the future. For example, if the total amount of fares were increased due to certain event, PyBer could use future events for promotion of their services.

3. **Urban cities have the highest ride and driver count** and **the lowest average fare per driver, that is $16.57**. I would suggest deeper research on this area by finding out what is the employee satisfaction rate and the company profit on this number (total fare amount is $39,854.38). If employee rate is high and PyBer is profitable, that would indicate a good bussiness strategy for urban cities. In addition, I would suggest to take a closer look into the peaks and dips that appear from late February to early April in order to find out what is causing them. This could reveal important information for future business planning. 

In this bussines proposal I have also included scatter plot that includes data per **each city within the city type** and reads **the average fare in correlation to total numbers of rides and drivers per city and city type**. The size of the bubbles correlates with **the driver count per city**. This visualization, besides the obvious disparities among the city types, suggest that looking into each city separetely could reveal important information about specific cities and aid to future bussines strategies.

<p align="center">  
<img src="Graphics/Fig1.png" width="50%" height="50%">
</p>
<p align="center">  
Ride-Sharing data in correlation to average fare to total number of rides and drivers per city type.
</p>

## References
(1) Module 5. The Matplotlib Library https://courses.bootcampspot.com/courses/200/pages/5-dot-1-2-the-matplotlib-library?module_item_id=59638, Trilogy Education Services,        2000, Web 13 Aug 2020.

(2) Customizing Matplotlib: Configurations and Stylesheets, Python Data Science Hand Book, https://jakevdp.github.io/PythonDataScienceHandbook/04.11-settings-and-stylesheets.html, Web 13 Aug 2020.

(3) Module 5. Plot a Pandas DataFrame and Series https://courses.bootcampspot.com/courses/200/pages/5-dot-1-10-plot-a-pandas-dataframe-and-series?module_item_id=59661, Trilogy Education Services, 2000, Web 13 Aug 2020.

(4)	Kaushik Mani, Introduction to Exploratory Data Analysis,  https://medium.com/datadriveninvestor/introduction-to-exploratory-data-analysis-682eb64063ff, Medium, Web 29 Jan 2019.

## Other Useful Articles
- [Matplotlib users guide]( https://matplotlib.org/3.2.2/users/index.html)
- [Create your Matplotlib style sheet in 10 minutes](https://hfstevance.com/blog/2019/7/22/matplotlib-style)
- [How to generate FTE Graphs in Python]( https://www.dataquest.io/blog/making-538-plots/)
- [Error Bars]( https://problemsolvingwithpython.com/06-Plotting-with-Matplotlib/06.07-Error-Bars/)


