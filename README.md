# Bike Shares project
This project is a programming assignment wherein I built a multiple linear regression model for the prediction of demand for shared bikes

## Table of Contents
* [General Info](#general-information)
* [Conclusions](#conclusions)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- Use Linear Regression to model the demand for shared bikes with the available independent variables

- A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state. 

- The company wants to know:
  + Which variables are significant in predicting the demand for shared bikes.
  + How well those variables describe the bike demands
- Based on various meteorological surveys and people's styles, the service provider firm has gathered a large dataset on daily bike demands across the American market based on some factors. 


## Conclusions
After doing the analysis, which contains EDA, Feature Selection, some categorical variables are found to have some impacts on demand of bike sharing:

Categorical columns that have positive impacts on demand are:
- weekday_Sun (from column weekday)
- Month 3, 6, 9, 10
It seems that people travel by sharing bike more on working day and Sunday.

Columns that have negative impacts on demand are:
- season_Spring (from column season)
- season_Winter (from column season)
- weathersit_Lightsnow (from column weathersit)
- weathersit_Mist (from column weathersit)
- Month 4 (from column mnth)

Combined with the columns has positive impacts, it seems that people use sharing bike less in Spring and Winter and when the weather is not encouraging (strong wind, snow, mist which reduce visibility)

The top 3 features that impacts 'label' column (demand of shared bikes) are:
- temp : coefficients of 3060.417 
- weathersit_Lightsnow: coefficients of -2544.739 
- yr_2019: coefficients of 2101.623 
