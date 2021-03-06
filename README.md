# Py-Ber_Analysis

Through the analysis of Pyber data, it is possible to determine statistics on the number of drivers, fare differences based on the rural, suburban and urban city types. Developing an analysis for these metrics can uncover the differences in demands of drivers and fares in specific communities throughout the first quarter of 2019. 
The data was analyzed using a variety of steps. It was first initiated by determining the total amount of rides, drivers and fares per city type. Determining the total amount of rides resulted in creating groups based on city types and summing them to obtain a total count of rides and drivers. This was similarly done to obtain the total fares for each city type. These results could then lead into the calculation of the average fare amount per ride in each city type as well as the average fare per driver. These results were finally displayed in a data frame to allow for ease of comparison. 

For the plot displaying total fares by city type, the Pyber data frame accounting for all cities in all city types was cleaned to display the Date column and plotting to create a selected column list accounting for fares, city types using the datetime index. A pivot table was then created to be able to log all city types within the data timelines and plotted for the analysis of trends. 
As the data was finalized, the stark contrast between city types in terms of fare, drivers and demand becomes apparent. In the summary data frame the amount of total rides for urban cities is about 13 times larger than rural cities. The amount of total drivers in urban cities is also 5 times higher than the suburban total drivers. The average fare per ride and average fare per driver trends determine the urban city has the lowest fare per ride in comparison to the other city types. When looking at the amount of drivers in the urban cities it is clear to see that because the amount of drivers in the urban cities is so high, the average fare per ride and average fare per driver are significantly cheaper than rural areas where drivers are more scarce and distances longer. This would ultimately mean that average fare per ride and fare per driver to be higher than more densely populated communities. 

![](https://github.com/bbar12/Py-Ber_Analysis/blob/master/analysis/SummaryDataFrame.PNG)

Fig 1. Summary Data Frame

As a preliminary analysis, this works well with the line graph as it more visually explains the finding. Something that the line graph determines more accurately is the decrease and increase of Pyber uses throughout the different city types throughout the months of January to April of 2019. This could more easily tell us the months affected by high demand and low driver demands. 

![](https://github.com/bbar12/Py-Ber_Analysis/blob/master/analysis/TotalFaresbyCityType.png)
Fig 2. Total Fares by City Type

Some of the challenges encountered were in making the date time index be recognized instead of as an index values so that the resample function could be performed. Performing a pivot table using Python as opposed to Excel was also less interactive and more like raw data handling. Overcoming the challenges meant visualizing at which data frames converting the index with the date/time to a datetime index to be able to perform the resample function successfully. Another challenge was to determine the syntax being used within my code and finding new syntax functions to implement not only for results, but clear enough for me to understand and retrofit into my analysis. This required a lot of preliminary visualization and heavy use of the  "print" function in jupyter notebook to visualize results as code was being retrofitted for obtaining specific results. 

Some recommendations I would give the CEO for addressing disparities among the city types is to determine the demand of rides that might be in demand for specific seasons and would recommend analysis into other months of the year, as this analysis only covers through April of 2019. 
Two additional analyses I could perform to gain more insight into the data are:
	- Looking into datasets throughout the year of 2018 as this might give historical Pyber data of demand and company growth. This could be done by creating a summary data frame as was done with 2019 and calculating percentage differences. 
	- Looking into datasets that expand throughout more cities in the US and comparing with our current analysis. This could be done through merging data frames and grouping values by not only city type but state as well. 
	- Creating line graphs of the current 2019 values against historical data to provide a historical projection of of Pyber ride-sharing performance. 
