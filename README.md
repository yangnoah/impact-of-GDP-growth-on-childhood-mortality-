# impact-of-GDP-growth-on-childhood-mortality-
An analysis of the impact of GDP growth on childhood mortality for countries around the world

This analysis used data from [Gapminder](https://www.gapminder.org/data/)

The question that this analysis looked at was:
What is the impact of GDP growth on childhood mortality for countries around the world?

## Analysis Steps for Question 1: 
1. A [dataset](https://github.com/yangnoah/impact-of-GDP-growth-on-childhood-mortality-/blob/master/Original%20Data.csv) behind an analysis of life expectancy vs childhood mortality was downloaded 
2. A [dataset](https://github.com/yangnoah/impact-of-GDP-growth-on-childhood-mortality-/blob/master/child_mortality_0_5_year_olds_dying_per_1000_born.csv) of childhood mortality for countries around the world was downloaded
3. The life expectancy data was removed from the working dataset
4. HLOOKUP was then used to search the childhood mortality data and import the numbers into the working dataset
5. The .csv was then imported into Jupyter Notebook and a Plotly animation was created. 

![alt text](https://github.com/yangnoah/impact-of-GDP-growth-on-childhood-mortality-/blob/master/ChildMort_GDP.JPG)

# What do these findings mean and why are they important? 
The results show that over time, childhood mortality is decreases as GDP increases. This makes sense because the wealthy a country is, the more resources it will have for healthcare and to take care of newborns. The opposite is also true which explains why childhood mortality is high for the poorest countries. 

What is surprising to note is that it seems like the same childhood mortality rate can be acheived under very different GDP conditions. This is important because it suggests that healthcare systems have similar childhood mortality outcome with very different levels of funding, suggesting that efficiency and delivery of care can be optimized. 

# Who might benefit from this analysis? 
This analysis is important to govenments of countries who are outliers. Countries like Saudi Arabia have childhood mortalities that are much higher than they should have based on their GDP. This suggests very high levels of inequality, poor funding of healthcare, or some other unexplained variable.

# Why was HLOOKUP in Excel used? 
Python is useful for handling datasets that are so enormous that they slow down Excel or cannot be reasonably manipulated in Excel. This dataset was not that large and having visual cues to inplement HLOOKUP was helpful. Python is good for Plotly animation which makes animation easy. This animation is not possible in Excel. 

# What data is needed for future analysis? 
Since GDP/person is just a proxy for healthcare expenditure, this analysis could draw stronger conclusions if healthcare spending per person was used instead of GDP/person. This could show which countries are truly inefficient with their spending. In the current analysis, it is possible that a country overpays significantly for their healthcare as a percentage of GDP but this is not obvious. 
