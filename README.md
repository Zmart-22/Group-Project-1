# Group-Project-1

Pynergy

As a group, we worked together to determine that we would like to review statistics associated with renewable energy resources within the state of Colorado. 

The questions that we wanted to answer was first, in recent history how has renewable energy stacked up against nonrenewable energy in Colorado? Secondly, based on the trends that we find, what is a projected outlook in the future for these energy sources during the same time frame moving forward? In our analysis, we used the previous 6 years and a projection of 6 years going forward.


Data Exploration
We found a variety of data sources and open APIs but found that many had data that was not applicable to our task or, in the case of Xcel Energy, the data was restricted and we were denied access. We were able to locate complete data to compare three main renewable energy sources: solar, wind, and hydroenergy. We compared these sources between themselves and additionally between major non-renewable sources: coal and natural gas. We found two major non-renewable sources in Colorado as the others sources are used minimally in the State. 

The main source we used for this analysis was the EIA (Environmental Impact Assessment). It contains large amounts of historical data for a variety of energy topics, including multiple energy sources and their usage throughout the United States by sector and states. 

-The API has years of information from both renewable and nonrenewable energy sources
-Used the requests.get() function to import API, then viewed data using json() and json.dumps() functions
-After reviewing with json.dumps formatting, we were easily able to visualize the data and also plan which data to specifically use for our studies

Data Cleanup
We filtered our requests to contain data from 2016-2021 by the individual energy source. We used the data we found to create scatter plots to show the evolution of use over time for each source. We included a regression line for each energy type to clearly show year over year change. Out of the five sources reviewed, solar, wind, and natural gas showed increases year over year 2016-2021 whereas coal and hydro use declined. 

-To narrow our API data down further, we utilized a for loop and the append () function to select the specific data our study required and add it to a list.
-Created multiple data frames using the information compiled within each list. We were able to then write csv files specific to energy type & calendar year. 
-As a result of great efforts in cleaning and filtering our data, we were quick and efficient to plot and analyze our results!


We also added two predictions for renewable and non-renewable energy sources. Based on the data we found, we predict that usage from three referenced renewable sources will continue to increase over the next 6 years while usage from the two referenced non-renewable sources will decline. 

For our findings in answering the questions that we had asked in our proposal, there were a couple main conclusions that we found with our data. First, over the course of the last 6 years, we have found that renewable energy on average has been continously increasing, as our nonrenewable energy has continued to decrease. 

![image](https://user-images.githubusercontent.com/125075891/230796407-a8e5a33d-5e4e-461b-b3a8-a82f453ea951.png).   ![image](https://user-images.githubusercontent.com/125075891/230796424-6bfdd41e-2c55-4826-9728-b787b8c2dac7.png)

Another major conclusion we found is that natural gas is still the mostly used energy source in Colorado, and until the last few years, that trend showed increases in usage. One of the factors that could have contributed in the spike of usage during the 2020 year could have been the pandemic in which the US has not seen the likes of.

![image](https://user-images.githubusercontent.com/125075891/230796432-6c110fae-28ae-483b-913b-55e78afeeccb.png)

One of the conclusions we found that was unexpected was the use of Hydro decreasing over the last 6 years. Because we saw that renewable energy has been increasing on average, we would not have expected the use of hyrdo to decrease like it has.

![image](https://user-images.githubusercontent.com/125075891/230796513-27e7eccd-2d3f-421a-9d88-a3a17112d990.png)


