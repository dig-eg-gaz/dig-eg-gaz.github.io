---
title: "Bubonic Plague"
authors: [OscarNaranjo]
date: 2019-12-09
categories: [analysis]
---

The goal of my post is to answer questions such as the reasons behind the spread of the Bubonic Plague across Egypt, what cities were the most affected and why, and what actions were taken to cease it. In doing so I will integrate charts and graphs of where and when occurrences were the most often. This information was gathered conducting an Xpath query on the Egyptian Gazette between the years 1904-1907. The following query will be used to search for words such as "plague", "bubonic", and "bubonic plague". The following Xpath query was included 
//div[@type="page"][@n="3" or @n="4" or @n="5"]/div[not(@type="advert") or (@type="advertisement")]/p

<iframe src="https://public.tableau.com/views/Bubonicplaguechartdata/Sheet2?:display_count=y&publish=yes&:origin=viz_share_link:showVizHome=no&:embed=true" align="center" width="90%" height="500"></iframe>
<iframe src="https://public.tableau.com/views/Bubonicplaguechartdata/Bargraph?:display_count=y&publish=yes&:origin=viz_share_link:showVizHome=no&:embed=true" align="center" width="90%" height="500"></iframe>

The goal of my post is to answer questions such as the reasons behind the spread of the Bubonic Plague across Egypt, what cities were the most affected and why, and what actions were taken to cease it. The answers to these questions will be collected from in-depth research within the pages of the Egyptian Gazette from the years 1905 and 1907. In doing so I will integrate charts and graphs of where and when occurrences were the most often. To conduct this research, formulating an Xpath query was necessary to produce results. Words such as "plague", "bubonic", and "bubonic plague" were put in _find/replace in files_ in Oxygen Editor restricting it to the following Xpath: **//div[@type="page"][@n="3" or @n="4" or @n="5" or @n="6"]/div[not(@type="advert") or (@type="advertisement")]/p**. What this Xpath query does is that it looks under the first two **div** located only in pages 3, 4, or 5 of the newspaper for a certain word or phrase inside a paragraph that must not be an ad. Knowing that pages one and two are full with ads and so are the last two, the xpath query ignores those pages.

However, doing just this will end in hundreds of thousands of useless results. Therefore, three different working sets were created which were configured to only include files from one year. In other words, the Xpath stated above was ran separately on each year. The outcome from this search then revealed useful information that was then applied to formulate graphs and maps shown below as well as theoretical responses to my questions regarding the Third Pandemic spread.

The earliest records of the Bubonic Plague within _The Egyptian Gazette_ was found on January second of 1905. However, according to history, the first outbreaks of the plague in Egypt took place back in April of 1899 after a long time of disease-free ([Plague In Egypt](www.jstor.org/stable/20436191.)). Here is a quick description from the _Egyptian Gazette_ itself of what the bubonic plague was, how it spread, and examples of incidents.
> "It appears from the report that I have received from Dr. Cresswell and from my own observations, (says Sir H. Pinching in his report) that these cases are due to infection conveyed by rats, which had been infected themselves by goods coming from India or Upper Egypt. One of the persons attacked by plague at Suez is an assistant in a shop, which contains large quantities of indigo coming from Calcutta and tea from Madras. In moving the cases containing these goods the dead bodies of rats were found." (1905-01-02.xml)

In spite of the exposure to the plague in other regions or nations, the economy and thus trade did not stop. The Egyptian government, did not want to interrupt trading among allies as it would cause severe economic problems ([Plague In Egypt](www.jstor.org/stable/20436191.)). After the terrifying news spread through the country, precautions were taken in ports of other countries, "A telegram from Constantinople of yesterday states that arrivals from Alexandria are submitted to a medical examination and disinfection, while rats on board ship must be destroyed"(1905-06-19). Based on my research throughout the newspaper, as you can see above, the way the Bubonic plague spread in Egypt was through the trade ports from Delta or Upper Egypt. Although rats are blamed here, it was actually through infected fleas humans got the plague as they sucked blood from the infected rats and then bit humans.

So when was this vast plague the worst? In other words when and where was it the most frequent. To answer these questions, lots of exhaustive research was performed. As previously stated, the words "plague", "bubonic", and "bubonic plague" were used in my query. After analyzing the text, the newspaper contained a section with weekly reports of the amount of incidents across Egypt as well as in other parts of the world, stories, and  more. The following bar graph was constructed using my findings.

(NOTE: Bar graph data not exact to real numbers, yet it is an accurate small-scale representation).
<iframe src="https://public.tableau.com/views/Bubonicplaguechartdata/Bargraph?:display_count=y&publish=yes&:origin=viz_share_link:showVizHome=no&:embed=true" align="center" width="90%" height="500"></iframe>


In comparison with 1904, as the bar graph shows, there was a considerable diminution in the number of cases of plague in Egypt as in the year of 1905. However, the following year, 1906, the plague spread and the number of cases severely increased. Real estimates are said to be the following:
> "The total number of cases notified since the beginning of the year amounted to 464 against 257 and 854 for the corresponding periods of 1905 and 1904 respectively." (1906-09-25.xml)

The plague has persisted in Egypt each year since 1899 arriving from the trade ports. With that said, that means that the cities closest to the ports must be the ones most affected by it. After gathering the following data through the _Egyptian Gazette_ and inputting it into Tableau, this statement proved to be correct.

(NOTE: Map data not exact to real numbers, yet it is an accurate small-scale representation).
<iframe src="https://public.tableau.com/views/Bubonicplaguechartdata/Sheet2?:display_count=y&publish=yes&:origin=viz_share_link:showVizHome=no&:embed=true" align="center" width="90%" height="500"></iframe>


As shown above, the city that was most frequently affected by the Bubonic Plague was Alexandria. Following Alexandria was Suez, which also has a huge trade port that connects the Red Sea with the Mediterranean Sea. However, after reading through the newspaper I encountered another possibility of why this might be the case.
> "It is the only town with a drainage system, and many of the drains are in a very dilapidated condition and infested with rats. This may be one of the reasons which account for the persistence of the disease at Alexandria" (1906-07-27.xml).

In regards to preventing the spread of this plague, “Clayton Gas” was used in the early 1900s. It destroyed not only rats and vermin, but also the parasites on them and sterilized the eggs of insects as well. Since no cures were discovered until 20 years later, preventions taken towards infected humans were unsuccessful. An important thing to notice is that the infected rat is the cause of the disease remaining endemic in a town, but the epidemic form of the disease is caused by the infected human being.
