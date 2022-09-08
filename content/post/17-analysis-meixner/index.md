---
title: "Patterns and Trends with Weddings"
authors: [MiaMeixner]
date: 2017-05-01
---
For my analysis project I decided to research weddings and their patterns and trends throughout the *Egyptian Gazette*. I ran many different XPath queries and got many different results, which I found to be very interesting. The wedding announcements were broken down into three main categories: military weddings, royal weddings, and regular or miscellaneous weddings. Most of these weddings are just announcements that the wedding is going to, or already has, happened.

# Military Weddings
Although military weddings are not the most prominent in the *Egyptian Gazette*, they are definitely mentioned. The people mentioned in these announcements are people of importance. Often generals, ambassadors, captains and more are the people who are fortunate enough to get mentioned in this newspaper. It makes sense that you must be an important, or well-known, person in order to be featured. However, the newspaper doesn't really touch on why these people are important. For example, this is a paragraph taken directly from the newspaper.

> A marriage has been arranged between Captain the Hon. Cuthbert James, Egyptian Army, second son of Lord and Lady Northbourne, and Florence elder daughter of Mr. and lady Alice Packe.

The most we know about this announcement is that the man is a part of the Egyptian Army and is the son of two important people. We see this because the *Gazette* mentions "Lord and Lady Northbourne" like they are well-known in society. We also see that the woman is the daughter of two important people also. We see this once again because the *Gazette* mentions "elder daughter of Mr. and lady Alice Packe" like it would be known who these people are. This is a common pattern throughout the *Gazette*. The newspaper will often mention people who are sons or daughters of more important people. Another instance of the *Gazette* mentioning someone's family tree is as follows.

> The marriage of Captain Kenrick, of the 11th Hussars, and Miss Helen Little is now fixed for April 29, at St. Mary Abbott’s, Kensington. The bride will be given away by her brother, Mr. Arthur Little (of the 20th Hussars), and the best man will be Major Bailey (of the 11th Hussars), who is the second son of Lord Glanusk.

Once again the *Gazette* mentions their family by saying "of the 11th Hussars" and "of the 20th Hussars". It also says "the second son of Lord Glanusk" which shows that the readers should just know who Lord Glanusk is. Based on these results, we can see that it isn't just enough to be a military captain or general. You must also be related to well-known people in some shape or form.

# Royal Weddings
This brings us to royal weddings. Even in the military section you can see that a lot of the generals or military personnel who are getting married are also related to someone who we can assume to be famous. Some of these famous people may actually be royalty. This section of weddings is the smallest of the sections because it is the most exclusive. Most of the people who are mentioned in this section are princes, princesses and people who are high up in the government. Many times in this newspaper it is hard to distinguish which category these weddings would fall into because they just mention the names of the people, like you are supposed to know who they are. For example, they mention "Mr. William H. Quintana" and we are just supposed to know why this man is famous. We can infer he is not in the military, otherwise he would have a title in front of his name. However, it is hard to identify if these people are just famous figures or royal figures. That is why most of the time you have to look for the title Princess or Prince. For example, the *Gazette* mentions...

>The marriage of Princess Margaret to the eldest son of the Crown Prince of Norway and Sweden will be that that throne, too, will course of time be occupied by a descendant of James I.

By this example we know that these people are a Prince and Princess because it is obviously stated. However, I noticed that they are royalty from Norway and Sweden. This makes me think that they only mention that people are royalty if it is outside of Egypt. This would make sense because you do not have to say that the Queen of Egypt is a Queen because if you live in Egypt, then you would already know that. This made my research much more difficult. Now, lets look at the weddings that don't fit into either category.

# Regular/Miscellaneous Weddings
This section is definitely the largest because it includes the most kinds of weddings. There are weddings of ordinary people, who may have actually paid to get their wedding announcement in the *Gazette*. An example of this is as follows.

>The marriage arranged between Miss Mary Prior and Mr. William H. E. Quintana will take place at St. Catherine's Cathedral Alexandria, on Monday, 24th inst., at 2 p.m.

This is just a simple wedding announcement, which doesn't show whether or not these people are actually important to society or not. You also have people who are just well-known or maybe even famous in the Egyptian community, whose wedding would be announced for the pure fact that they are celebrities and the Egyptian people are curious about their lives. An example of this kind of wedding is as follows.

>The marriage of Mr. Dormoy, chief engineer of the Suez Canal Company’s ateliers, to Mlle Kirchesner was celebrated last evening at the Church of St. Eugenie, in the presence of the Governor, who is an intimate friend of both families, and many, if not all, the chiefs of the Suez Canal Company, besides a large concourse of other friends. A largely attended reception was held afterwards at the Continental Hotel, and the festivities were kept up to a late hour.

In this announcement you can tell the two people themselves are well-known because they are "chief engineer of the Suez Canal Company's ateliers". Also you can tell these people are important because the governor himself came to their wedding. Finally, you have people who themselves aren't very well-known, but their families are extremely well-known. An example is as follows.

>A marriage has been arranged between Horace Montague Rumbold, second secretary at the British Agency, Cairo, eldest son of the Right Hon. Sir Horace Rumbold, Bart, G.C.B. G.C.M.G., and Etheldred Constantia, second daughter of the late Sir Edmund Fane, K.C.M.G. and Lay Fane of Boyton, Wilts.

We see that these people are very well-known through their families. The *Gazette* posted "eldest son of the Right Hon." and "second daughter of the late Sir Edmund Fane" which shows to the readers that those people themselves are nobodies, but the readers should know who their family is. Once again, it is difficult to tell exactly why these people are famous, because the *Gazette* doesn't say exactly how, it is just implied that they are well-known.

# Marriages Throughout the Months
Another thing I wanted to research was which months do most of the weddings that are mentioned in the *Egyptian Gazette* take place. I ran the XPath query `//div[@type="page"]//p[contains(.,"marriage")]`. When I ran this query I got every single section in the *Egyptian Gazette* that mentions a marriage, no matter what it says about that marriage. I wanted to see how many times marriages are announced in each month every year. I found that in 1905 numbers were generally higher from the months of May-June. This makes sense because many people like to have summer weddings over winter weddings. I also noticed that the numbers in 1905 were much higher than the numbers in 1906, which makes me think 1906 may have had many weddings announced under something else other than "marriage". In my visual, you can see these patterns and you can tell that 1906 had much less numbers than 1905. This makes me curious to know if maybe the people who did the editions in 1906 just messed up, or if there really weren't as many weddings in the whole year of 1906. Maybe the *Egyptian Gazette* even started to not report these weddings as much. My research also showed me that in 1906 November and December had no marriages at all mentioned. This to me shows that maybe nobody was assigned these months, or if they were maybe only a few people and the whole issues for those months weren't finished.

![Marriages Announced per Month/Year](MarriagesAnnouncePerMonth-Year.png)

# Conclusion
Overall, there are three types of marriages that are reported on in the *Egyptian Gazette*. These are military weddings, royal weddings, and regular or miscellaneous weddings. Also, we can see from these queries is that summer months are more popular to have weddings, for obvious reasons. One final thing we can conclude is that in 1905 the *Gazette* reported far more weddings than in 1906. We may never know exactly why that is, but that could be something we further research at another time.
