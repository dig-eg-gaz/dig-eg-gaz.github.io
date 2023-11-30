---
title: "Hotels in Cairo"
date: 2017-04-16
authors: [KailenChapple]
categories: [analysis]
---
## What hotels were visited the most in Cairo Egypt?

![Hotels in Cairo between 1905-1906](chapple-map-screenshot.png)
[Link to live map](https://www.google.com/maps/@30.0302842,31.1812774,13z/data=!3m1!4b1!4m2!6m1!1s1DunCjoyI8KrRBpKhOk1C7EDsJijzv3J3)

### Social and Cultural

From my results, I was able to find that in the summer months the amount of visitors visiting the hotels increased. In Egypt tourism became a vital part of the Egyptian economy after the construction of the Suez Canal had been completed. The hotels included in my results are all along the Nile River and the opening of the Suez canal made it much easier for people to get in and out of Egypt from around the world.

>"During the second half of the nineteenth century, a new system had emerged, one that would subsequently be applied to Egypt and Sudan. The new centerpiece of this new structure was the 'Resort'. Resorts were dedicated to tourists".

### Querying Results and Haptics

The query that I used to find the hotels listed in Cairo is Query: `//div[@type="advert"][contains(., "Cairo”)]/head` and in text to find I put "Hotel". Finding the query that would give me the answers that I wanted took me a long time. I initially asked myself where I would be able to find hotels in Cairo within the Digital Gazette. The answer that I came up was in the advertisements section, Local and General, and the Social sections of the issues. I began by trying to run the query `//div[@type="advert"]` that would give me the titles of all of the hotels within the advertisements section. This was unsuccessful because the query was not answering my question of what the most common hotels in Cairo were. The query that I was running was not specific enough toward the location and gave far too many results to decipher. The next query I began to run was specific, however it was far too specific when trying to answer my questions because it did not give me any results. Many of the queries I tried to run failed because some of the results were in element or feature, which made it hard to find a full set of data. The biggest issue that I ran into was being specific enough to generate a query, but not too specific where I would get a small number of results. After trial and error, I was able to finally retrieve the query Query: `//div[@type="advert"][contains(., "Cairo”)]/head` with the text finding the word hotel. This query finds an advertisement that contains the word Cairo in the head and hotel somewhere in the text. This query is not perfect, however it did assist me in answering the question that I posed.

The query that I was able to retrieve for the hotels answered my question of what hotels in Cairo existed in Colonial Egypt, however this query still did not give me an accurate representation of the people who attended these hotels. I further had to construe a query that would answer the question of who visited the hotels and when the people visited these hotels. When coming up with a query to answer this question, I discovered the element: "visitList". When making a query for visitList, this was difficult because I wanted to make the results specific, yet attainable. I began with the query of Query: `//div[@element="visitList"]`, this query gave me results that stated yes, meaning that that there was a visitList element in the issue. I needed to make the element much more specific. I generated the query `//div[@element="visitList"//persName]`. This did not give me results as it still was not specific enough. I generated results to find persName within the visitList attribute with using regular expression `\W\w+ \W\w+`. This regular expression would give me the results for people within the visitList that were tagged with persName. The results for this test came up for me, however many people that coded for the _Egyptian Gazette_ in XPath did not use this tag. I generated results for only a couple of dates.

[Visitors in Cairo Egypt in 1905](https://public.tableau.com/views/visitList/Story1?:showVizHome=no&:embed=true)

<iframe src="https://public.tableau.com/views/visitList/Story1?:showVizHome=no&:embed=true" align="center" width="90%" height="500"></iframe>

The strengths that I found with using Xpath and generating results using regular expression were that it was able to find a specific answer for me if I asked it the right question, however if I asked the right question some of the results would not populate if others did not put on their end the same exact XML markdown.

### References
When thinking about a topic such as hotels in Egypt, it is important to find scholarly reviewed text for a more accurate understanding of the topic at hand. I was able to find three articles to assist me in answering the question about tourism and hotels within Cairo.[_THE THOMAS COOK ARCHIVE FOR THE STUDY OF TOURISM IN NORTH AFRICA AND THE MIDDLE EAST_](http://www.jstor.org/stable/23062746?Search=yes&resultItemClick=true&searchText=hotel&searchText=colonial&searchText=Egypt&searchUri=%2Faction%2FdoAdvancedSearch%3Ff1%3Dall%26amp%3Bf3%3Dall%26amp%3Bq1%3Dcolonial%2BEgypt%2B%26amp%3Bacc%3Don%26amp%3Bed%3D%26amp%3Bsd%3D%26amp%3Bc3%3DAND%26amp%3Bq0%3Dhotel%2B%26amp%3Bgroup%3Dnone%26amp%3Bc6%3DAND%26amp%3Bq2%3D%26amp%3Bf4%3Dall%26amp%3Bc1%3DAND%26amp%3Bf2%3Dall%26amp%3Bf5%3Dall%26amp%3Bf6%3Dall%26amp%3Bf0%3Dall%26amp%3Bq3%3D%26amp%3Bisbn%3D%26amp%3Bq5%3D%26amp%3Bpt%3D%26amp%3Bq6%3D%26amp%3Bc4%3DAND%26amp%3Bc2%3DAND%26amp%3Bq4%3D%26amp%3Bc5%3DAND%26amp%3Bla%3D&refreqid=search%3Adb8b6213b82816d7b3da77e796434632&seq=1#page_scan_tab_contents)
explains how tourism in the Middle East and North Africa took a dramatic incline during the 1880s. The essay details how “Mass tourism is synonymous with the name of Thomas Cook and Son Ltd.” Thomas Cook and Son Ltd. helped pave the way for tourist coming in and out of Egypt after they developed “the Nile transit service while simultaneously opening up Syria/Palestine to travelers.” This information is important because it explains why the hotels included in this visualization were popular during their prime. The visualization depicts five hotels in Cairo, and all but one of these hotels are all situated near the Nile River.

Another scholarly article that I have used as reference is [_Tourism and Empire: The Thomas Cook & Son Enterprise on the Nile, 1868-1914_](http://www.jstor.org/stable/4289940?Search=yes&resultItemClick=true&searchText=hotel&searchText=colonial&searchText=Egypt&searchUri=%2Faction%2FdoAdvancedSearch%3Ff3%3Dall%26amp%3Bf6%3Dall%26amp%3Bc1%3DAND%26amp%3Bed%3D%26amp%3Bq0%3Dhotel%2B%26amp%3Bacc%3Don%26amp%3Bf4%3Dall%26amp%3BcurrentPath%3D%252Faction%252FdoAdvancedSearch%26amp%3Bf2%3Dall%26amp%3Bpage%3D2%26amp%3Bsd%3D%26amp%3BsearchType%3DfacetSearch%26amp%3Bf0%3Dall%26amp%3Bf1%3Dall%26amp%3Bc5%3DAND%26amp%3Bc2%3DAND%26amp%3Bc3%3DAND%26amp%3Bc6%3DAND%26amp%3Bc4%3DAND%26amp%3Bgroup%3Dnone%26amp%3Bf5%3Dall%26amp%3Bq1%3Dcolonial%2BEgypt%2B&seq=1#page_scan_tab_contents). This article details how tourism is a widely Western phenomena. "A product of the industrial revolution, modern tourism was founded, developed, and perfected in Britain, western Europe, and North America during the second half of the nineteenth century". Tourism in Egypt was a new concept during the early twentieth century. This concept is important to think about and analyze within the Digital Gazette because the citizens of Cairo and neighboring cities like Alexandria were trying to understand tourism as a means to stimulate their economy.