# P1_energy_water_analysis

##### Project Title: Energy and Water Consumption Analysis for Buildings in LA

**Team Members:** Yash Kansal, Meera G K, Yeyan Wang, Crystal Wang, Shweta Joshi

**Project Description/Outline:** We will be analyzing the Socrata Energy and Water Consumption open source data for the City of Los Angeles. We will be focusing on different buildings across the City of LA and try to understand which factors contribute most to energy and water use consumption in the buildings and in turn, which levers could be used by the city to reduce the said consumptions.

**Research Questions to Answer:**
Question 1: Which 5 property types have the highest correlation between Water Use and Carbon Emissions, and Source Energy Use Intensity (Source EUI) and Carbon Emissions?
Question 2: What property type has highest source energy use intensity and water use per square footage for buildings built after the year of 2000?
Question 3: Does any property type have a correlation between Water Use and Gross Building Floor Area (GFA), and if there is a correlation, what is the relationship between for building type with highest correlation value?
Question 4: For multi-family housing building type, check if there is a relationship between year built and source EUI, as well as year built and water use per square foot? 

**Dataset Link:** https://dev.socrata.com/foundry/data.lacity.org/9yda-i4ya

Analysis:
1)	Pull dataframe and create a new dataframe that only includes columns needed and drop rows with the NaN and "Not Available" values
2)	Change the data type to float for columns with number values
3)	Find out number of buildings for each property type and determine which property types have at least 300 data points so the data is not affected by rarely occurring properties
4)	Create a new data frame with only highly frequent property types

For Question 1: 
1)	Make scatter plot and display linear regression line on plot and create a DataFrame which shows the correlation between Carbon emissions and other variables (Water Consumption and Source EUI). 
2)	Display the top highly correlated property types for water consumption vs. Carbon Dioxide Emissions
3)	Display the top highly correlated property types for source EUI vs. Carbon Dioxide Emissions
4)	Create dataframe for plotting
5)	Show plotting for results
![image](https://user-images.githubusercontent.com/116146774/215669260-c0e7c787-7a7a-4993-9e13-2533af04d319.png)
![image](https://user-images.githubusercontent.com/116146774/215669494-b66baa13-d89f-4f76-b6c5-9036dc017026.png)

 
For Question 2: 
1)	Create another dataframe only columns we will need to find water use for each building type and show buildings built only after 2000
2)	Find out which building type has the highest water consumption and highest source energy consumption using groupby 
3)	Use bar plot show the graph. 

![image](https://user-images.githubusercontent.com/118711472/215361310-843b1dd4-3b51-4533-b6d4-9dec5d72d41f.png)
![image](https://user-images.githubusercontent.com/118711472/215361314-3d93fc6d-b69a-4152-b865-980912b38063.png)
   

For Question 3: 
1)	Find the correlation between water use and gross building floor area for different building types
2)	Print the building type with the highest correlation between water use and gross building floor area
3)	Plot the correlation values for different building type
4)	Plot Gross Building Floor Area vs Water Use for Manufacturing/Industrial Plants
![image](https://user-images.githubusercontent.com/118711472/215361327-2331e3ed-e32c-4d41-93b7-a639cf6a35ae.png)
![image](https://user-images.githubusercontent.com/118711472/215361342-19263fa0-d725-48d9-828b-4b9933c452a1.png)

 

For Question 4: 
1)	Create bins for year built column
2)	Divide water use by property gross footage area and filter dataframe by Multifamily housing
3)	Calculate median for each bin using groupby
4)	Use line plot to obtain the answers. 

![image](https://user-images.githubusercontent.com/118711472/215361362-b3661350-b06a-4920-a42e-445a176867d2.png)
![image](https://user-images.githubusercontent.com/118711472/215361369-82a7ea05-4541-45af-8706-af3f171616a0.png)
   

Conclusions:
1)	For source energy use and carbon emissions, there appears to be a very strong positive correlation for Retail Stores, where the correlation coefficient between the two variables is 0.9830449798002524.
2)	Medical Office has the highest energy consumption per sq-ft, with a value of 168.6 kgal/sq-ft for buildings built after 2000. Hotel has the highest water consumption per sq-ft, with a value of 8115.6 kgal/sq-ft for building built after 2000.
3)	For water use and gross building floor area, there appears to be a moderately strong positive correlation for Manufacturing/Industrial Plants, where the correlation coefficient between the two variables is 0.5215937191397046.
4)	The water usage intensity has decreased with year the property was built, however, no such trend is observed for energy use intensity.



