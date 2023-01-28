# P1_energy_water_analysis
This repo is used to record Project 1 for Team 7 of UCB Data Analytics Bootcamp (2022-23)

Project Title: Energy and Water Consumption Analysis for Buildings in LA

Team Members: Yash Kansal, Meera G K, Yeyan Wang, Crystal Wang, Shweta Joshi

Project Description/Outline: We will be analyzing the Socrata Energy and Water Consumption open source data for the City of Los Angeles. We will be focusing on different buildings across the City of LA and try to understand which factors contribute most to energy and water use consumption in the buildings and in turn, which levers could be used by the city to reduce the said consumptions.

Research Questions to Answer:
Question 1: Which 5 property types have the highest correlation between water use, and carbon emissions and source energy use and carbon emissions?
Question 2: What property type has highest source EUI consumption and water consumption per square foot for buildings built after 2000?
Question 3: Does any property type have a correlation between water use and gross building floor area, and if there is a correlation, what is the relationship between water use and gross building floor area for that building type?
Question 4: For multi-family housing building type, is there a relationship between year built and source EUI, as well as year built water consumption per square foot?

Dataset Link: https://dev.socrata.com/foundry/data.lacity.org/9yda-i4ya

Breakdown of Tasks:
Get the data from the API.
Save the data as Pandas dataframe.
Clean the dataset.
Discuss which columns and groupings are required for each question.
Create specific sub-datasets for each question.
Create figures (data visualization such as line graph, bar chart, etc.) to analyze the relationships and comparisons.
Draw conclusions from the results.
Write a summary report.
Create a Google Slide Presentation.

Analysis:
For Question 1: 


For Question 2: first we find out water usage per square foot for all building type for all year, then only look at the dataframe for year built after 2000, find out which building type has the highest water consumption using groupby and then using bar plot show the graph. Same steps for finding the highest source energy consumption for year built after 2000. 

  ![image](https://user-images.githubusercontent.com/118711472/215296585-ddcd8ea5-b542-40f0-bbd4-24a2916a7c1b.png)
  ![image](https://user-images.githubusercontent.com/118711472/215296589-849bd5cf-5418-43f4-9f0e-c9cabfddb698.png)

For Question 3: 

For Question 4: first we create bins for year built column, then dividing water use by property gross footage area, filter dataframe by Multifamily housing, calculating median for each bin using groupby, and then using line plot to obtain the answers. 
   ![image](https://user-images.githubusercontent.com/118711472/215296554-dde8398c-c00f-4875-b8a1-ad5f3ed848a7.png)
   ![image](https://user-images.githubusercontent.com/118711472/215296561-12757186-9cc3-4dd5-aed5-cf8a39542876.png)


Conclusions:

