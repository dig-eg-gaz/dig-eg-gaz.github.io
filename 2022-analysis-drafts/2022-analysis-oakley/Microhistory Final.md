---
title: "What is the Cultural Significance of Mummies in Early 20th Century Egypt?"
subtitle: "insert"
summary: "insert"
authors: McKennaOakley
tags: ["insert"]
categories: [analysis]
date: 2022-12-02
featured: false
draft: false
projects: 

---
Research Question (and what specifically sparked my interest in my topic from the Gazette)
---
Prior to my learning in this course, the only Egyptological concept I was somewhat familiar with was that of the mummy. Mummies are the remains of humans or animals that have been preserved through special ceremonial practices, such as the removal of internal organs and the wrapping of their bodies with bandages. Growing up in a modern culture of Western civilization, I was exposed to mummies at museums, in history textbooks, and in countless movies, TV shows, and books like *Goosebumps*. I never learned about them in-depth, though, and they seemed to always just be exploited for their "creepy" factor rather than their cultural significance.

Already faintly accustomed to this disparity in mummy representation, I was especially shocked when I realized that after encoding several issues of the *Egyptian Gazette* I had not read a single mention of mummies. Based on the stereotypical portrayals of Egyptian cultures in Western media, there should have been plentiful discussions of mummies in the *Gazette*. This gap between stereotypical expectations and reality intrigued me, and I instantly wanted to know more about mummies and their true significance in Egyptian culture beyond Hollywood films. With all this in mind, I decided to explore "What was the cultural significance of mummies in early 20th century Egypt?" as my research question. I limited the scope of my findings to the early 20th century to better utilize our course's repository of *Gazette* records.

Queries & Visualizations
---
I began my research with the following X-Path query:
--* //div[matches(.,'mummy', 'i')]/@feature

I started with this relatively broad query to find which features the word "mummy" was mentioned in, hoping I could notice some trends that would then help me to narrow my research down even more. Based on the results from this query, I was able to create the following data visualization.
image: ![Mentions of the Word "Mummy" In Any Feature](1st-Query-Visualization-jpg)
  focal_point: "Smart"
  preview_only: true
The query only yielded eleven issues with features that mentioned the word "mummy," but based on the results, I found that "mummy" occurred most times on the third pages of issues. From here, I could refine my next XPath query to hopefully get more results, and to get a starting point for my actual analysis.

My second query to focus on the page number was:
--* //div[@type="page"][@n="3"]//div[matches(.,'mummy', 'i')]
image: ![Mentions of "Mummy" Over the Years](2nd-Query-Visualization-jpg)
  focal_point: "Smart"
  preview_only: true

This query yielded 37 articles that mentioned the word "mummy." Based on the visualization, I could see that mentions of the word "mummy" were higher in 1905, and gradually decreased to 1908, although there was a slight spike in mentions in 1907. Not only could I analyze the quantity of mentions, but this query gave me a small pool of articles I could read to help me answer my research question. This query gave me more resources because it yielded *all* mentions of the word "mummy" on my specified page number rather than the ones that fell under specific features, like in the first query. I found this query to be far more efficient as a starting point for my actual analysis as it gave me more material to work with. 

Based on some of the trends I noted in the articles, it seems that at this point in Egyptian--and world--history, mummies are more of a cultural spectacle for other countries than a sacred practice for native Egyptians in preparation for the afterlife as it used to be. Hence, most articles talk about mummies in relation to museum exhibits or the projects of American Egyptologists. Similarly, other articles talk about European collectors of mummies and the easy accessibility of mummies (1907-10-03 issue). Then, there are the couple of articles talking about the sketch “The Mummy and the Mummer” written and performed by an Englishman, which further exemplifies the spectacle-nature of mummies to non-Egyptian cultures. (I will be heavily revising and adding more to this paragraph, these are more just my notes.)


Supplementary Research
---
These are some of the secondary sources I have found that I will concisely explain and relate back to my personal findings with the *Gazette*. I haven't gotten around to doing it yet, but will very soon!

["Between Spectacle and Science: Margaret Murray and the Tomb of the Two Brothers"](https://www.cambridge.org/core/journals/science-in-context/article/between-spectacle-and-science-margaret-murray-and-the-tomb-of-the-two-brothers/BD9BF4396C3C3AEE6CD594BAB2E5BA73)

["Unswathing the Mummy: Body, Knowledge, and Writing in Gautier’s Le Roman de la momie"](https://muse.jhu.edu/article/184522)

["Unwrapping the Past: Egyptian Mummies on Show"](https://www.cambridge.org/core/books/abs/popular-exhibitions-science-and-showmanship-18401910/unwrapping-the-past-egyptian-mummies-on-show/F68462C54FA7D5FAC336412E3AB36F9E)

Conclusion
---
Here I will conclude and summarize my analysis, and I will reflect on the strengths and weaknesses of my digital research methods.

Works Cited
---
Lyu, Claire. “Unswathing the Mummy: Body, Knowledge, and Writing in Gautieris Le Roman De La Momie.” Nineteenth Century French Studies, vol. 33, no. 3, 2005, pp. 308–319., https://doi.org/10.1353/ncf.2005.0026. 


Rogers, Beverley. “Unwrapping the Past: Egyptian Mummies on Show.” Popular Exhibitions, Science and Showmanship, 1840–1910, 2015, pp. 215–234., https://doi.org/10.4324/.9781315655123-19. 

Sheppard, Kathleen L. “Between Spectacle and Science: Margaret Murray and The Tomb of the Two Brothers.” Science in Context, vol. 25, no. 4, 2012, pp. 525–549., https://doi.org/10.1017/s0269889712000221. 