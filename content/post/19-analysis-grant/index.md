---
title: "Railway Accidents from 1905-1907"
authors: [DamianGrant]
date: 2019-12-05
categories: [analysis]
---
In the Egyptian Gazette, I came across many instances of rail-related accidents. The seemingly prevalent issue caught my attention and initiated my analysis on railway accidents reported in the Egyptian Gazette from 1905-1907. This analysis attempts to add to the knowledge and research on this topic by looking at the geographical locations of rail accidents reported, the types of rail accidents reported on, and when during the year these accidents occurred. I will then use my findings and the research of others to contextualize these rail accidents, looking at how railway development and their workers have been reported on in the Egyptian Gazette, and the, perhaps, limited scope that this provides.

## Research Methods

Before my analysis, I will briefly explain some of my research methods. To compile the data set used for this analysis, I used the XPath query: `//div//head[matches(.,'accident','i')]/following-sibling::p[matches(.,'train','i')]` to search for all articles with a headline containing the word "accident" and a paragraph containing the word "train." This search gave me 47 results. To create as complete a data set as possible, I tried several variation of this search, which resulted in seven more articles. After excluding irrelevant articles, I ultimately resulted in a data set of 32 railway accidents reported in the Egyptian Gazette from 1905-1907. This data served as the core for my analysis.

## Geographical Locations

In looking at the locations of railway accidents reported on, the overwhelming majority, 26 out of 32, occurred within Egypt, with 11 being reported under the “Local and General” feature. This suggests that the people reading the Egyptian Gazette cared more about that which pertained to them and their locale than they cared about events unrelated to themselves, when it came to railway accidents. However, international accidents were reported on too. Specifically, six of the 32 reported on occurred outside of Egypt (Sudan, Syria, Israel, France, England x2 ). These international events often involved royalty, or someone else of wealth, or was a tragic event, such as the death of dozens of people or a child. Other than England and France, the other countries reported on were in close proximity to Egypt. The inclusion of these two European countries demonstrates the newspaper’s audience’s connection to colonial Britain. I have mapped all the reported railway accidents to the best of my ability. This involved updating some city names to their modern spellings and marking all accidents found in “Local and General” as occurring in Alexandria. These approximations seem accurate as one can nearly trace a line between the locations in and around the Nile Delta, many of which follow along water ways or in clear paths, indicating that a rail line may have existed there. 

<iframe src="https://public.tableau.com/views/TrainAccidents/LocationalPrevalenceReportedOn?:showVizHome=no&:embed=true" align="center" width="90%" height="500"></iframe>

## Types of Accidents

There were four main types of accidents reported on. Those caused by a crash, derailment, unfastened door, or, the most prevalent of those reported, someone being run over. In the bar graph below, one can see the number of times each type of accident was reported on over the three years, broken down by the outcome of that accident: No Injuries, Injury, or Death. Cases where there were both injuries and deaths were counted as a “Death.” This breakdown shows that most of the accidents reported on resulted in an injury or worse. Most of the “No Injuries” were crashes or derailments of goods trains. Also frequently mentioned, was the delay that the accident caused, such as on September 15, 1905 when a train derailed, resulting in “an hour and twenty minutes late in arrival in Alexandria.” This further demonstrates the idea that what is considered newsworthy is that with dramatic outcomes or an impact to one’s daily life.

<iframe src="https://public.tableau.com/views/TrainAccidents/NumberofTimesTypesofAccidentsareReported?:showVizHome=no&:embed=true" align="center" width="90%" height="500"></iframe>

## Monthly Prevalence

I also investigated when these accidents occurred and their prevalence in the newspaper at that time. To prevent results skewed by one year simply having more or less issues, I graphed the number of accidents reported divided by the total number of issues for that month to find the fraction of issues that contain a reference to a railway accident. This resulted in the following graph that shows spikes and falls, but does not reveal a common trend. Perhaps if all the months contained fuller daily data, a clearer trend would appear.

<iframe src="https://public.tableau.com/views/TrainAccidents-ReportingFrequency/ReportingFrequency?:showVizHome=no&:embed=true" align="center" width="90%" height="500"></iframe>

## Contextualization and Final Analysis

When I started my research I was expecting an overwhelming disapproval or blame of railway workers for these accidents. This assumption came from my early findings on workers being reported as [“careless”](https://dig-eg-gaz.github.io/post/2019-10-17-damiangrant/) and from Ziad Fahmy’s published journal entry in which he states that, “The general feeling of disenfranchisement, … were subtly blamed on British wartime rationing and foreign-owned capital,” such as the railways. However, this was not clearly confirmed nor denied.

There were many instances of railway workers’ deaths being mentioned briefly and without much regard, which may indicate a lack of empathy or care for this group of people. But, this was also common throughout the paper for other people as well. There were also instances in which railway workers were talked about with respect, such as when they did a good job caring for the first-class after the derailment of a sleeping car or when the driver of a train broke his arm. Rather than showing a consistent, strong feeling towards railway workers, these instances hint at an important class distinction, in which events relating to the upper-class get more publicity and detailed writing, while the working-class and others do not receive the same coverage.

While analyzing the Egyptian Gazette gives insight into Alexandria at the turn of the century, it is important to note that it is just one point of view from a diverse city. The ease of transportation granted by railways enabled British colonialism over Egypt during this time, something many Egyptian Gazette readers likely were aware of. As explained by On Barak, these transportation lines were so essential that a series of strikes in 1919 which “paralyzed transportation inside and between cities” caused “British rule in its current form” to become “impossible.” It would be interesting to see how railway workers and rail-related accidents were reported on in other newspapers, particularly those not designed for a British, English speaking audience. I predict that there would be greater negative coverage of railway workers and accidents as a form of criticism and disapproval of British control in Egypt.

## Sources

On Barak, “Scraping the Surface: The Techno-Politics of Modern Streets in Turn-of-Twentieth-Century AlexandriaPreview the document,” Mediterranean Historical Review 24, no. 2 (December 2009): 187–205.

Ziad Fahmy, “Media-Capitalism: Colloquial Mass Culture and Nationalism in Egypt, 1908-18Preview the document,” International Journal of Middle East Studies 42, no. 1 (2010): 83–103.