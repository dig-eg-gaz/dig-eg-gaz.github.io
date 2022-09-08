---
title: "Maximum and Minimum Temperature in Alexandria, Egypt (May 1906-April 1907)"
authors: [AlainHernandez]
date: 2019-12-01
categories: [analysis]
---
### Introduction
Over the last few decades, the topic of global warming has gotten huge publicity all around the world. This analysis was created with the purpose of finding out whether or not global warming has been occuring specifically in Alexandria, Egypt by taking data found from May 1906 to April 1907 and comparing it to an article I found that lists the temperature change in Alexandria Egypt over the last 100 years to see if there has been an increase in the average temeperature and if so what could be the leading factors in the climate change.
### XPath Query
The Xpath Queries I have chosen to use are: 
1.Max Temps: //table//cell[contains(.,'Max. Temp in the shade')]/following-sibling::cell[1]/number()  
2.Min Temps: //table//cell[contains(.,'Min. Temp in the shade')]/following-sibling::cell[1]/number()

The goal of the query is to find a certain table in the newspaper which shows the weather information  which typically is found on page 2-3 and from that, I would take the data that is under the maximum  and minimum temperature section. By taking the following sibling cell after the cell that says max temperature and minimum temperature, I will be able to gather the numbers provided and copy and paste them into Atom to then use them to create useful visualizations. The Xpath query had to be narrowed down to keywords such as the exact titles of the weather report or else the information could be skewed. Another important thing in making the query was making sure that the results that were given back were in numbers so it would not mess up the graph if someone would have written something in that section.

### Data Visualization
Since the data I have gathered was far too large to display one by one on the bar graph, I had to split it up into months and show the average temperature of each month. While looking through the data individually, I found that there were very few giant errors in the numbers provided which made the graphs look a lot smoother than if otherwise it had a giant spike out of nowhere. From the graphs we can interpret that the temperature reaches its peak in July and goes through a steady decline until february and after february it starts to increase back up and keeps following this cycle. When looking at the minimum temperature it looks a little odd how it goes from a steady decrease from July to November, then a huge drop in December and then goes back up in January and then declines again afterwards. It is a very confusing pattern. It may have to do because of the lack of dates around the time which lead to a skewed average or just a cold front.
<iframe src="https://prod-useast-a.online.tableau.com/t/alainhernandez/views/MaxTemperature/Sheet1?:showVizHome=no&:embed=true" align="center" width="90%" height="500"></iframe>


<iframe src="https://prod-useast-a.online.tableau.com/t/alainhernandez/views/mintemperature/Sheet1?:showVizHome=no&:embed=true" align="center" width="90%" height="500"></iframe>


### Significance of the Data

The data found in this Xpath query was useful in trying to find out the patterns of temperature in Alexandria Egypt over the span of a year. This data gave a clearer picture of how the climate in Egypt didn't change drastically since of its geographical location being in the desert. It never really got too cold but you could a gradual decrease in temperature over the winter time and gradual increase in temperature over the summer time. This data will be useful in determining whether or not these patterns are supported by an outside source that probably has more accurate information on the subject.
### Historical Context
[Temperature Patterns in Egypt over the past 100 years](https://www.researchgate.net/figure/Seasonal-temperature-trends-and-Mann-Kendall-test-for-trend-Z-test-and-rate-of_tbl2_303018027)
This article shows the trends of temperature from 1900 to 2010 in Alexandria, Egypt and other parts of Egypt. This article shows the bigger picture of the climate change that has been happening in Egypt using a larger sample size than the one we used in the analysis project.
To make a conclusion about global warming being present in my data would be difficult to do because the data I have is limited and I don't have enough data to show the change from one year to another so my sample size is very limited in what it represents but it works with the article I have provided to show the bigger picture of how a gradual increase of temeprature has been occuring in certain areas of Egypt in every single season. 
### Research Remarks

After doing this research, there were a few remarks that I would like to point out regarding the accuracy of a given data element and how that can ultimately skew your research. Initially, as I began constructing my XPath Query, as I've discussed before, the data isn't always perfect. The query did not yield results for every single day in all 3 years. The results were dense in the earlier years but as time went by, that data began to thin out, making it very difficult to pick apart data that can accurately represent what I am trying to research. Even though the data that was presented, yielded, some of the measures were wrong, due to human error. For me, as I was dealing with averages across each month, the human error threw my data visualization off-proportion, in which I had to change. I am by no means saying that these digital methods of acquiring data are bad. In fact, the ability to use a query to yield results from various newspapers over several years is very efficient. However, a weakness of researching through digital methods is that the data presented isn't always accurate, questioning the validity and accuracy of the research itself. Furthermore, the data could be missing, also highlighting the inaccuracy of the data element.