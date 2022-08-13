# surfs_up

## Overview of the Analaysis
Our client W. Avy is considering opening a surf and ice creaam shop in Oahu. To determine if this is a business that is sustainable year-round we are conducting analysis on Temperature data. We focused our analysis on analysis on two specific months: June and December. 

### Data Sources and Software
To conduct our analysis we were provided with weather station data for Hawaii. The data was provided as a sqlite database and it contained two tables: 
 - measurement
 - station

The analysis was conducted in python using the following dependencies:
 - numpy
 - pandas
 - sqlalchemy 


## Results
The results of the analysis are shown below.

### Summary Statistics for June
The main points determined in the analysis of the month of June are:
 - Total Readings: 1,700
 - Mean Temperature: 75
 - Minimum Temperature: 64
 - Maximum Temperature: 85 

The table below shows the complete summary statistics for the temperature analysis for the month of June. 

![june_summary](https://github.com/kkoehn8/surfs_up/blob/main/Images/JuneTemperatures.PNG)

### Summary Statistics for December
The main points determined in the analysis of the month of December are:
 - Total Readings: 1,517
 - Mean Temperature: 71
 - Minimum Temperature: 56
 - Maximum Temperature: 83 

The table below shows the complete summary statistics for the temperature analysis for the month of December. 

![dec_summary](https://github.com/kkoehn8/surfs_up/blob/main/Images/DecemberTemperature.PNG)

When comparing the summary statistics for June and December we can see the following results:
 - While there are fewer total readings for December the numbers are comparable
 - The Mean Temperature is similar, it's on 4 degrees cooler in December
 - The Minimum Temperature shows a greater variance with the minimum temperature in December being 8 degrees cooler
 - The Maximum Temperature is similar, it's only 2 degrees higher in June

## Summary
The analysis should be useful for our client W. Avy to make a decision if the ice cream and surf shop is sustainable year-round. The analysis shows that the mean temperature between the two months (June and December) is above 70 degrees with only a 4 degree lower mean in December. However, if our client wants additional information to help him make his decision he may want to consider the following analyses that could be conducted:
 - Analysis for a specific station: The analysis we conducted was for all 9 stations in Oahu and there could be regional differences on the Island. If W. Avy has an idea of where on Oahu he wants to locate his ice crean and surf shop we could refine the analysis by focusing on that specific station instead of all stations on Oahu. If W. Avy doesn't have a specific location in mind, grouping the analysis by station may help point him to a specific location that may do better. 
 - June and December analysis per year: The sqlite database contains readings from 01/01/2010 to 08/23/2017. The analysis we conducted was for the entire dataset, there could be variations over the year and it could point to a trend. Conducting the analysis for June and December of 2010, June and December of 2011, up to June and December of 2015 may show us how things are changing over time. By showing that over the years the mean temperature is decreasing or increasing W. Avy may feel more comfortabe making a decision.
