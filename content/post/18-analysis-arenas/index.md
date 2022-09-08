---
title: "Attitudes towards Germany: Random, Situational, or Seasonal?"
date: 2018-05-07
authors: [DanielArenas]
categories: [analysis]
---
1905 was a watershed year in the period preceding WWI. Tensions ran high as Russia was in the process of earning the distinct honor of being the first European nation to lose a war to a non-Western power (Japan), and the great powers were concerned if this, and the nascent but ultimately futile 1905 revolution, meant the decline of Russia as a major imperial power, which would certainly throw the delicate balance of alliances into chaos. But more sensationally, and closer to home, the German Kaiser Wilhelm II openly challenged French claims to incorporate Morocco into their sphere of influence, encouraging the Sultan Abdelaziz to convene an international conference to decide the fate of the kingdom. This is the age of sensationalist press too, where newspapers did not just report news, but had the power to make it as well. Journals mattered, and were a vital means of measuring (or controlling) public opinion, an invaluable tool for historians. Precisely when newspapers are at their yellow-journalistic, propagandic worse is when they hold the most value. The decisions of what stories to run, and how they are written reveal quite a lot about the mindset, values, and beliefs of not just the publishers, but their readership as well.

As the main English newspaper in colonial Egypt, the _Gazette_ should roughly represent the overall average of British views, but what surprised me the most working on my week was the sheer variety of opinions, and none felt so jarringly dissimilar as those concerning Germany. With this project, I sought to find out whether there was a discernable pattern in when the _Gazette_ published editorial articles critical or supportive of Germany, and for the most part it seems there is none, and changes in the frequency follow events in the news.

## Methodology and Structure
This investigation sought to do two things; quantify a subjective piece of data (occurrence of a pro- or anti- Germany article), collect the data, and observe whether any patterns emerged.

The biggest potential fault of this investigation comes from the very beginning: how to measure what is an article’s stance on Germany? From the start I wanted to look at one thing in particular, not wires/telegrams, but articles. These were difficult to isolate because in the newspaper itself there is little regularity in which these appear and how they are presented, which means that in the encoded library it becomes that much more difficult to find them.

To do this, I used the following xpath queries:
- `//div[@type=”article”]//p[contains(.,”Germany”)]`
- `//div[@type=”item”]//p[contains(.,”Germany”)]`

This is a bit of a “needle in a haystack” approach. I couldn't use `@element="wire"` because that would have only brought up results such as news telegrams, which do not contain the expression of opinion I was looking for. Nor am I sure would more specific queries have gotten me better results, because as mentioned above, what I am looking for is not always classified in the same way, and its page location can vary wildly (especially in 8 page issues).

I went through these results (which contained many lines from standardized ads or referencing ship arrivals), and read the articles to determine its position. This is unfortunately the most subjective part of the process and thus the one most open to error. I classified any opinion article as pro- or anti- based on two factors. One was whether the article (and being published by the _Gazette_ arguable the newspaper itself) considered the government or state of Germany as a threat either to the perspective of the writer of the article or as threatening to a third party (and not always a military threat, and it was rarely such an outright sentiment of fear or anger), and whether the article held sympathy for or encouraged the success of the German government or state. Both of these are because what would often happen is that the article would extol the virtues of the “German” while decrying his government, most often in the context of the supposed “failure” of the German state to maintain her colonial empire up to “correct” standards. Germans would be portrayed as successful despite coming from Germany, rather than because of it, which I took as a solid indicator of anti-German sentiment. But again, this is the most subjective part of the process, and I could not succeed in standardizing these criteria any deeper than that. It became a question of “you know it when you see it.” In any case, once I identified an article, I would go into the div header and add the phrase `ana=”#german-positive”` or `ana=”#german-negative”`. I then ran the queries again to limit the results of the searches to just the articles I intended to use.

I kept my data confined to the year 1905 to limit the number of results. That year alone provided me with almost 100 articles. An interesting further avenue of research is if we can see a gradual change in opinion over the course of years.

Once I collected the results of these two xpath queries I copy/pasted them into Atom, and by using regular expressions cleaned up the data until each point was just two variables: date, and either positive or negative.

I then went into tableau, and organized the data into two charts, each measuring the results over the course of 1905 by quarter and month. One shows the comparison between positive and negative articles by type:

<iframe src="https://public.tableau.com/views/DanielArenasChartComparisonByType/Sheet1?:showVizHome=no&:embed=true" align="center" width="90%" height="500"></iframe>

The other measures the frequency of each type of article in a much clearer way:

<iframe src="https://public.tableau.com/views/DanielArenasChartComparisonByFrequency/Sheet1?:showVizHome=no&:embed=true" align="center" width="90%" height="500"></iframe>

## Analysis

What does this data show us? Ultimately, not much. The only patterns that can be discerned is that articles of both types spike randomly, following events, not pre-determined patterns as was previously thought, and that consistently the _Egyptian Gazette_ agreed with Grey’s Foreign Office in considering Germany (usually in conjunction with the Ottoman Empire) as a threat to British interests. It must be noted however, that there is also a consistent publication of pro-German articles, showing that while the imperial agents in Alexandria more or less “toed the line” with the government, this was not universal. Even though a good deal of these pro articles came from German newspapers (as opposed to English or other continental ones for the anti side), their universal publication in English rather than the alternative French which likely would have been more popularly spoken among the other European citizens in Alexandria, could suggest that there was a minority among the British imperial agents in support.

While there may not be much to show for it, I do believe this question of the representation of Germany in colonial newspapers is intriguing, and well worth further exploration. The two biggest problems facing such future work are the lack of a standardized way to define an article’s position, and with the paper itself: its lack of regularity with these opinion based articles that do not come from Reuter’s or Havas means that they are more difficult to search for in xpath, as they will be encoded in many different ways in the collection itself.
