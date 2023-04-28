# Where Are Chicagoans Going?

## Table of contents
* [Tableau Dashboard](#tableau-dashboard)
* [Motivation](#motivation)
* [Data Questions](#data-questions)
* [Data Sources](#data-sources)
* [Cleaning the Data](#cleaning-the-data)
* [Problems and Hurdles](#problems-and-hurdles)
* [Technologies Used](#technologies-used)
* [Insights](#insights)


## Tableau Dashboard
https://public.tableau.com/views/WhereAreChicagoansGoing/Story1?:language=en-US&publish=yes&:display_count=n&:origin=viz_share_link

## Motivation
As a resident of a city that does not have many public transportation options, I tend to make assumptions about the accessibility to public transit that residents in larger cities have and how that affects their habits. When I visited Chicago last year, it seemed like there was public transportation everywhere I looked. I’m curious about whether Chicagoans use private modes of transportation when public transportation is available.

## Data Questions
	- Which areas are people using private transportation to get to and from most frequently? 
	- Are those routes served by public transportation?

## Data Sources
The following data sources were used in this project:

	- Rental Bicycle Data from Divvy (https://divvy-tripdata.s3.amazonaws.com/index.html)
	
	- Chicago’s Open Data Site:
	
		○ Private Transportation Datasets:
		
			§ Transportation Network Providers (Rideshare) Trips (https://data.cityofchicago.org/Transportation/Transportation-Network-Providers-Trips-2018-2022-/m6dm-c72p)
			
			§ Taxi Trips (https://data.cityofchicago.org/Transportation/Taxi-Trips/wrvz-psew)
			
		○ Public Transportation Datasets:
		
			§ Bus Routes (https://data.cityofchicago.org/Transportation/CTA-Bus-Routes-Shapefile/d5bx-dr8z)
			
			§ Bus Stops (https://data.cityofchicago.org/Transportation/CTA-Bus-Stops-Shapefile/pxug-u72f)
			
			§ L-Rail Lines (https://data.cityofchicago.org/Transportation/CTA-L-Rail-Lines-Shapefile/53r7-y88m)
			
			§ L-Rail Stations (https://data.cityofchicago.org/dataset/CTA-L-Rail-Stations-Shapefile/vmyy-m9qj)
			
			§ Metra Lines (https://data.cityofchicago.org/Transportation/Metra-Lines/q8wx-dznq)
			
			§ Metra Stations (https://data.cityofchicago.org/Transportation/Metra-Stations/nqm8-q2ym)
			
		○ Zip Code Boundaries (https://data.cityofchicago.org/Facilities-Geographic-Boundaries/Boundaries-ZIP-Codes/gdcf-axmw)
	

## Cleaning the Data
Trips meeting the following criteria were used for this analysis:
	- A beginning timestamp in 2022
	- Over 2 Miles (or an estimate was used based on trip duration)
	- Under 1 Day
	- Origin and destination in different zip codes

## Problems and Hurdles
The trip datasets are massive. Specifically, the rideshare dataset contained almost 70 million rows for 2022. The data had to be processed in batches and then reconsolidated.

## Technologies Used
	- Python for exploration, cleaning, and aggregating
	- Tableau for dashboarding
	- PowerPoint for presentation (the Tableau Story should be referred to for the "Findings" section)
	- Git for version control

## Insights
Despite access to public transportation along the same routes, many people still choose to use private transportation methods to get around Chicago. There is room for improvement in the city's public transportation offerings that may encourage more usage.
