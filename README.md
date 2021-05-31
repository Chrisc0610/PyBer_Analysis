# PyBer_Analysis

## Overview of Project
The purpose  of this analysis is to create a new Data Frame out of the ride-sharing data by city type.
to achieve this I will use the same csv's that we were given by Omar. After getting the output of the DataFrame
a mutiple line graph was created to visiualize the data of Total Fare by City Type.

## Results
The results for the new DataFrame are explained in more detail below. 

- Merging the cvs's into a new DataFrame and getting total counts. 
	* I merged the two CSV's provided by Omar and got the counts for the follwing: the total rides, total drivers, total fares. 
		- I started by merging the CSV's and creating a new DataFrame called "pyber_data_df" the image below shows how I merged the data.
	* [Merged DataFrame](Resources/NewPyber_dataframe.PNG)	
	
	* After creating the new DataFrame i got the total counts I needed as well as Total Average Fare per Ride and Driver.
		- I used the "groupby" function to get the total counts for the total rides, total drivers, total fares. The image below shows how I got 
		each count and total averages.
	* [Total Counts](Resources/Total_counts_F_D_R.PNG)	
	
		- I got the Total Average Fare per Ride and Driver by dividing the series of total_fare_count by total_ride_count and total_fare_count by total_driver_count.
	* [Total Averages](Resources/Total_averages.PNG)	
		
	* Finally I created a new DataFrame from all the data above, refer to the steps and images below.
		- Once the Data Frame was created I removed the index and changed the the columns to provide the Image below.
	* [New Summary DataFrame](Resources/new_sumary_DF.png)	
		

- Plotting the Dataframe to visiualize the difference in total fare by city type. 
	* I used the "groupby" function again to get a total fare count from the previous pyber_data_df. 
	* [Total Fare DataFrame](Resources/total_fare_DF.PNG)
		- Once I got the total fare count I created a pivot table to change the DataFrame table orientation.
	* [New Summary DataFrame](Resources/PivotofnewDF.PNG)		
		- Then I used a "loc" function to get a set of dates from our recent table
		- Then I used the "resample" function to create a new DataFrame that gets the sum by week and plotted the DataFrame,
	* [Function to Create plot](Resources/createplot.PNG)			

	
## Summary

	* After Analysing the data I can conclude the following. Please refer to the following pictures for this summary.
	
	* [New Summary DataFrame](Resources/new_sumary_DF.png)	
	
	* [Total City by Fare Type](Resources/PyBer_fare_summary.PNG)	
	
		- The Average Fare per Driver is the most expensive in a Rural city type. some of the factors that attribute to this is 
		the fact that there are a low amount of drivers (total of 78) as compared to the Suruban (total of 625) and Urban (total of 1625) city types. 
		- A solution to this could be getting more drivers out in the rural city types this would bring the cost of fares per driver while increasing
		the amount of total fares to compete to Suburban and Urban City types.
		- We can also see that in the month of March the is a spike and fall for each week in the Urban city types.
		- This can attribute as to why there is such a high amount of total fares in the Urban area.
		- Based of our Line Plot we can see that aproaching summer the total amount in fares in the Suburban city types increases.
	
		
