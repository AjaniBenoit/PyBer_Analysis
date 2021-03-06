# PyBer Analaysis

Analysis of rideshare data using Matplotlib

## Overview of Project 

Matplotlib was used to complete an analysis of data and create visualizations of the data for PyBer, a ridesharing app company valued at $2.3 billion. The analysis was completed on data provided from two excel file by PyBer. [city_data.csv]( https://github.com/AjaniBenoit/PyBer_Analysis/blob/main/city_data.csv) and [ride_data.csv]( https://github.com/AjaniBenoit/PyBer_Analysis/blob/main/ride_data.csv). Analysis of the data files primarily focused on an exploratory analysis of the data 

### Purpose 

The purpose of this report is to provide a summary of the findings from the exploratory analysis of the data.

## Results 

### Summary of Exploratory Analysis

The ride data and city data dataset were merged into one dataset using the Pandas merge function. The groupby() function was then used to calculate the total rides by city type; total drivers for each city type; the total amount of fares for each city type; the average fare per ride for each city type; and the average fare per driver for each city type. A new data frame was created to summarize the data.  
![summary_df.png]( https://github.com/AjaniBenoit/PyBer_Analysis/blob/main/summary_df.png)

An exploratory analysis of the data revealed the following:

1.	Drivers from rural cities had the highest average fare per ride and the highest average fare per driver. urban cities had the lowest average fare per ride and average fare per driver.
2.	Urban cities had the highest total rides; the highest total fares; and highest total number of drivers. Rural cities had the lowest number of total rides; the lowest total fares; and the lowest total number of drivers. 
3.	The total number of drivers in urban cities outnumbered the total number of rides.

#### Total Fare by City Type 

The groupby() function was used to group city type and date and calculate the sum of the fares from the merged Pyber data frame. A new data frame was created. The pivot function was used on the new data frame to set the date as the index for the data frame. The data frame was further manipulated with the weeks grouped to show the total fares by city type before being plotted into a line chart.
![Fig8.png]( https://github.com/AjaniBenoit/PyBer_Analysis/blob/main/Fig8.png)

The line chart plots fares in USD along the Y axis and the months along the X axis for each city type.The fares for Suburban and Urban cities peak in the latter part of February. Rural cities fares peak in April.

### Summary

1.	The average fare per ride was highest in rural cities and lowest in urban cities. Data on mileage driven should be include to determine if there is a correlation between the average fare per ride and miles driven. 
2.	Urban cities had more drivers than total number of rides and the lowest average fare per driver. Additional analysis will need to be completed to determine if there is a correlation total rides and total drivers on average fare per driver. 
3.	It is recommended that PyBer either focus on increasing the total number of rides in urban cities or reduce the number of drivers in urban cities. 
4.	Further data and analysis should be collected and completed to determine if there are any factors that contribute to total rides being lower than total drivers in urban cities

