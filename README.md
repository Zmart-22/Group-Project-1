# Group-Project-1

<img width="288" alt="logo" src="https://user-images.githubusercontent.com/125621763/231316246-657e3411-2327-489c-9003-e0d54a168461.png">

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

We were then able to clean the data further from our API results using for loops and DataFrames to create lists and repeated this process for all of the different types of energy.

From here we then created csv files for each of the energy sources analyzed for the years under review. These filtered csv files allowed for ease in creating visualizations of the results.

![jasoncode](https://user-images.githubusercontent.com/125621763/231316372-f0edccc3-80bd-4d3b-bcd1-413855a36076.jpg)

![csvscreated](https://user-images.githubusercontent.com/125621763/231316406-6d51d7ed-d0bd-463e-9e27-f0fa276f71a1.jpg)

Analysis Process

-We used the data we cleaned and made regression models and used the r value to find if there were any correlation in our energy sources


-We also used the month over month data to determine seasonal trending year by year for the renewable energy sources


-We then took our data and projected models of 6 more years into the future for the reviewed energy sources


Visualizations of our Results

HYDROELECTRIC

Hydroelectric use in Colorado has declined steadily on average over the last 6 years. It has the smallest percentage of use of the three larger renewable energy sources in Colorado.

![hyrdroyears](https://user-images.githubusercontent.com/125621763/231316545-c595d3da-fe00-48ce-8fef-1e18f903c0bb.jpg)


![hydromonths](https://user-images.githubusercontent.com/125621763/231316550-76e660d8-0dc9-471f-b3b7-97914558a6c3.jpg)


In a review of the hydroelectric use month over month, the usage increases through the early months of the year with a drop off generally in mid to late summer. This may be based on the seasonality of the energy source in Colorado based on climate.

WIND

-Wind power is the largest renewable energy source in Colorado. Its use continues to grow year over year with no indication of waning.

![windyears](https://user-images.githubusercontent.com/125621763/231316710-5dd9992c-c8c2-458c-8ab3-3e9c117245ae.png | width=100 height=100)


![windmonths](https://user-images.githubusercontent.com/125621763/231316600-cdef6be3-98ba-4644-a160-cbae14252c46.jpg)

-Wind has a usage pattern distinct from hydroelectric, as it sees a decline over the spring to summer months while usage increases in fall and winter. This may again be based on Colorado's changing seasons and weather patterns.

SOLAR 

-Solar power has shown a steady increase over the last 6 years in Colorado. There was a large increase between 2020 and 2021 possibly indicating that this energy source will continue to grow as a viable source for years to come.

![solaryears](https://user-images.githubusercontent.com/125621763/231316797-1da22400-1919-4e45-895a-4ad6ef6089a5.jpg)

![solarmonths](https://user-images.githubusercontent.com/125621763/231316819-d4d5685e-2e10-4bab-a8b9-aec7dc2c3d39.jpg)

-As with the other two reviewed renewable energy sources, solar usage is based on season trends month over month in Colorado. Solar usage increase through the spring and summer months with a sharp decline in the fall. Because solar has a smaller percentage of total renewable use, the variations month over month appear much larger than the other sources.

NON RENEWABLE

![coal](https://user-images.githubusercontent.com/125621763/231316882-d5c520d8-5fd5-42ec-90af-1dffaadcf335.jpg)


![natgas](https://user-images.githubusercontent.com/125621763/231316909-98c2f376-76e5-4432-ade0-f734ce3de509.png)


-As energy generated from coal continues to decrease over time, it seems natural gas continues increase.

-The decline of energy generated from coal is more drastic than the climb of energy produced from natural gas. 

LOOKING INTO THE FUTURE

![forcastrenew](https://user-images.githubusercontent.com/125621763/231317182-f17c5767-86eb-4f19-8e31-39348c52ecd2.jpg)

![forcastnonrenew](https://user-images.githubusercontent.com/125621763/231317164-82e3b7b5-6336-4583-97ce-da03f5e5ef8c.jpg)

We also added two predictions for renewable and non-renewable energy sources. Based on the data we found, we predict that usage from three referenced renewable sources will continue to increase over the next 6 years while usage from the two referenced non-renewable sources will decline. 

For our findings in answering the questions that we had asked in our proposal, there were a couple main conclusions that we found with our data. First, over the course of the last 6 years, we have found that renewable energy on average has been continously increasing, as our nonrenewable energy has continued to decrease. 

We can state generation of renewable energy will increase over time as non renewable decreases, however we project that energy generated from non renewable sources will account for even a  bigger percentage in the future.

![piehistory](https://user-images.githubusercontent.com/125621763/231317247-74866144-34c5-4c1b-883b-28cda233900c.png)

![piefuture](https://user-images.githubusercontent.com/125621763/231317236-3460f665-0285-46e9-967d-f3f1603199c6.jpg)

Another major conclusion we found is that natural gas is still the mostly used energy source in Colorado, and until the last few years, that trend showed increases in usage. One of the factors that could have contributed in the spike of usage during the 2020 year could have been the pandemic in which the US has not seen the likes of.

![image](https://user-images.githubusercontent.com/125075891/230796432-6c110fae-28ae-483b-913b-55e78afeeccb.png)

One of the conclusions we found that was unexpected was the use of Hydro decreasing over the last 6 years. Because we saw that renewable energy has been increasing on average, we would not have expected the use of hyrdo to decrease like it has.

Summary and Conclusions


-We were able to find results for the questions we asked and we saw that renewable energy use has increased over the last 6 years on average while on average nonrenewable energy has decreased

-Though wind and solar usages increased, we did find that hydro usage has actually decreased over the last 6 years showing a continuous decrease

-Natural gas use still continues to be the energy source mostly used, though in 2021 and future projects showing that trend may change as renewable energy continues to gain traction

-Due to the recent increase in natural gas, our future modeling shows that renewable energy will account for a less percentage of total energy over the next 6 years. The increase in natural gas use is greater than the increase in renewable energy



Numerical Summary

-Most of our data was collected in different quantity types, so for transparency we wanted to show all of our data in gigawatt hours which to us was easier to read than Trillion BTU’s. This was a conversion of 1 Trillion BTU’s is equivalent to 293.0710701 gigawatt hours

-According to the numbers, we had a positive correlation between time and renewable energy of an r value of 0.94 while we had a negative correlation between time nonrenewable energy with an r value of -0.80

-Comparing the mean between renewable and nonrenewable we see that over the course of the last 6 years, renewable consumption was sitting at 11,344.57 gigawatt hours while nonrenewable was around 40,902.04 gigawatt hours

-Next we compared the median between renewable and nonrenewable energy and we found that renewable energy was at 11,419 gigawatt hours and nonrenewable energy was 41,330 gigawatt hours

-Comparing the top nonrenewable energy (natural gas) and the top renewable energy (wind), we see quite a difference in production. Natural gas over the last 6 years has a max production of 18,171 and gigawatt hours while wind only had a max of 15,125 gigawatt hours



What do our findings mean?

-Colorado as a whole is starting to increase renewable energy use more and in correlation nonrenewable energy has started to decrease

-Natural gas still reigns king, but there are possible trends to show this could be reversing

-We have more questions we can start asking such as: What is the reason for a decrease in hydro use in Colorado? Do the trends of renewable and nonrenewable energy continue across the United States as it does in Colorado? What other factors may contribute to the rise and fall of certain energy uses?
