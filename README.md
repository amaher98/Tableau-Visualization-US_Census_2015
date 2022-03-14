# Tableau-Visualization-US_Census_2015

## Introduction
I am interested in socio-economic aspects and thus I chose the 2015 US Census Demographic Data to work on. 
The first 4 tabs in the workbook are considered the requirement of the project. The workbook consists of a dashboard that incorporates the last seven (7) worksheets, and three other worksheets that are standalone.


## Link
https://public.tableau.com/views/census_16471908693210/Dashboard?:language=en-US&publish=yes&:display_count=n&:origin=viz_share_link


## Discussion

My visualizations give insight on three questions:

#### 1.	How does income and poverty look across the states of the USA?

The dashboard consists of three visualizations, and they are filtered using the ‘State’ filter. 
The first three visualizations, located in the top left corner, show the population, unemployment rate and poverty rate. Whereas the population is calculated using a ‘sum’ aggregate function, the rates are calculated using an ‘avg’ aggregate function. 
The fourth visualization is the map of the US that show the average unemployment rate for each state. The scale is a gradient blue color; from light blue to dark blue as the unemployment rate increases. The map also shows the poverty rate as the user hovers over the states of selection. 
The fifth visualization is a bar chart, sorted from highest to lowest average income per capita. The bars show the poverty rate as well as the unemployment rate as the user hovers over the states of selection. Also shown on the visualization the unemployment rate as labels, to highlight their values easily as the user views the income.
The sixth and seventh visualizations are scatter plots that aim to examine if there is a correlation between the unemployment and the ethnicity of the population. This is shown through plotting the unemployment rate once versus the percent of the ‘White’ population and once versus the percent of all the other races, combined. With the exception of Puerto Rico, there seems to be no correlation between the unemployment rate and the non-White combined population percent. Puerto Rico is considered an outlier in this analysis since its White population is a small minority.   

 
#### 2.	What are the counties that have high average income per capita and high poverty at the same time?

It may be an interesting for socio-economic studies to understand where the highest gap between the average income per capita and the poverty rate. I chose to examine this at the counties level, since the states will not give useful information due to the high variation of both the income and the poverty among its different counties.
I applied a condition to filter the counties based on the average income being more than $30K and the poverty rate being more than 15%. The criterion I proposed is only based on the census data, and therefore, it is a subjective criterion. 
A total of fifteen (15) counties satisfies the criteria I made. New York county is the top county with an average income per capita of nearly $65K and a poverty rate of almost 18%. Having only 15 counties under this criterion could indicate that in general, there is no big gap between the average income per capita and the poverty rate across the US counties. 
I chose a bar chart that sort the counties based on the average income per capita. The bar chart shows the poverty rate as labels on each bar, as well as the unemployment as the user hovers over the counties.


#### 3.	How does the transportation system in the populous counties compare to each other?

I created two visualizations to show the mean commute time and the transit system use percent, respectively, for different counties. 
The mean commute time, shown by a bar chart sorted from the least time, can be a measure of the good traffic condition in the county. I developed a criterion to identify the counties that are populous, being the ones with population over 500,000 residents and that had short mean commute time being less than 21 minutes. This is done through creating a set from the ‘County’ column with the condition being its filter. Although, the choice of the thresholds of the population size and the commute time is subjective, the conclusion of identifying the populous counties with the least congested traffic remains reasonably sound. The bar chart shows also the population and the transit use when the user hovers over the bars.
The use of the transit system can be used as another measure of how good the transportation system is. I developed a criterion to select the populous counties (over 500,000 residents) with the transit system use of more than 10%. I created a set of those counties from the ‘County’ column. Seventeen (17) counties satisfy the criterion. I showed the counties on a bar chart, sorted from highest to lowest in transit use percent. The visualization also shows the population as the user hovers over the bars.
What is interesting is that, based on the criteria I used, no county appears in both groups. In other words, the counties that have the most use of transit system are not the one with least congested traffic condition. This finding makes sense, as people tend to use the transit system if the traffic is busy.
