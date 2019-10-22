# DS5500-HW2

## Problem 2
I choose Thomas Carpenito's visualization.[Link](https://github.com/Tommyixi/DS-5500-Homework/tree/master/HW1). Generally speaking, this visualization effectively visualize the distribution of income across countries. You can see income distribution across the world for different years. This one is pretty different with mine, as mine is static line plot, while his is dynamic map-form visualization which is very fancy. However, when talking about is it easy to interpret, his work needs some improvements. First, his visualization shows a general picture of GDP per capita all over the world. But his visualization only has 7 levels of GDP, namely 0 to 60000. You can only tell that a country belongs to a certain level and don't know an approximate number. Second, the color he chose need to be more distinguishable. I mean if you look at this plot, the entire Eurasia & African continent seems to be all blue, except for some pink in western Europe. Maybe changing the color would help to interpret more easily.

## Problem 3
I choose Noah Demoes' work. [Link](https://github.com/noahdemoes/DS5500_Homework1). Generally speaking, this visualization is pretty similar to mine, as we are both static line plots and we both effectively visualize it. Noah gives the income situation for all continents and all countries seperately, while mine gives a world's summed situation. His visualization is easy to interpret. You can find everything you need in the given question: GDP across countries and continents. However, for his plot for countries, it is a kind of messy that you can hardly ever distinguish the country you want to look at. This is due to the limitation of this kind of simple line plot. And the color for different countries is also hard to distinguish.

## Problem 4
This is a regression task. I choose Linear Regression as the model to quantify the relationship between income and life expectancy over time. Because we just need to investigate the relationship between three variables and the data we have is not much, plus intuitively income is correlated to life expectancy, I think the classic Linear Regession might be the solution. So I fit the Linear Regression model with the data (life expectancy as the target and `[income, time]` as the design matrix). I first use the plain income data but then find out the result is not ideal. So I did a log transform to the income data. The model achieved a R^2 score of 0.78 and RMSE of 7.8. This proves that Linear Regression is a decent model for this problem, though the result can be improved.

![vis](https://github.com/stiangithub/DS5500-HW2/blob/master/pr4.png)

There are 4 subplots, each represents a time period (I found out it is pretty messy to put all years into one plot, so I divide the time into 4 periods, which looks much better). The X axis is logged income and Y axis is life expectancy. You can see clear positive linear relationship between income and life expectancy. As for the time factor, the locations of most points move from bottom left to top right gradually. So I can say that time is positively related to both life expectancy and income. It is a reasonable result, since as people become richer, they are likely to put more money to help themselves to get healthier, which leads to the increase of life expectancy.

## Problem 4
Similar with problem 4, this is also a regression task to find out the relationship (intuitively it is a negative relationship) between income and child mortality overtime. I still choose the Linear Regression as the model because that there are only three variables and the data is not complicated. After setting the child mortality as the target, [income, time] as the design matrix, the Linear Regression model gives a result which has R^2 of 0.79 and RMSE of 77.9. Still, Linear Regression achieves a satisfactory result.

![vis](https://github.com/stiangithub/DS5500-HW2/blob/master/pr5.png)

The visualization contains 4 subplots, as I split the time into 4 major periods: 19th century, 1900-1950, 1950-2000, and after 2000. I first tried embed time into one plot but found out it was too messy. It is a good option to split time into 4 periods, as people can see the trend that child mortality is decreasing while income is increasing as the time goes. After all, we can see a clear negative correlation between income and child mortality over time. It is very reasonable that with the growth of income, people can put more money into caring children's health, which leads to the decrease of child mortality.


