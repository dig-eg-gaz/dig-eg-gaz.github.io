---
title: "Sudden Death in 20th Century Egypt"
authors: [ElenaBeggs]
tags: ["PE-RU-NA", "catarrh", "Dr. William's Pink Pills", "Allenburys'", "sickness"]
date: 2022-12-02 
categories: [analysis]
---

I began the research by searching for a correlation between illnesses and patent medicine advertisements. This led me to research the types of illness the medicine advertisements claimed to cure. The final question I decided to research is: whether illnesses mentioned in the _Egyptian Gazette_ are comparable modern illnesses of the same name. I compiled a list of the most common diseases mentioned in the _Egyptian Gazette_, but in the end, catarrh was the sickness about which I was most curious. The three companies I considered were Peruna, Allenburys’, and Dr. William’s Pink Pills. 

Peruna is a very familiar sight in the _Egyptian Gazette_. Overwhelmingly, Peruna promised to cure catarrh and consumption. Peruna referenced catarrh as a sickness, “Peruna is the best remedy for all catarrhal diseases. When the catarrh has become systemic, – that is, when it has been allowed to spread through the entire system, it is a difficult disease to cure” (“PE-RU-NA was successful where doctors failed”, June 26, 1906). By reading the quote from the newspaper, it is apparent that the authors of the advertisement thought of catarrh as a disease. Today, the term catarrh is not as prolific. Its meaning is also more ambiguous. The definition of catarrh according to Merriam-Webster is an “inflammation of a mucous membrane” (Catarrh). Peruna claims catarrh can be of the head, throat, lungs, stomach, kidneys, and pelvic organs. According to the _British Medical Journal_ from 1859, the symptoms of catarrh are: grit in the eye, headache, impairment of smell, thirst, appetite loss, nausea, and abdominal pain ([Jones](http://www.jstor.org/stable/25193777), p.773). The Sudafed® website lists these symptoms of catarrh: runny nose, headache, face pains, feeling of mucus in the throat, “a reduced sense of smell and taste, temporary hearing loss and a crackling in [the] ear, and a sore, scratchy throat” ("[What is Catarrh](https://www.sudafed.co.uk/what-catarrh-and-how-get-rid-it)"). It is very difficult to find any information about catarrh in a modern sense. These two lists of symptoms are very similar. The main difference is the catarrh mentioned in the _Egyptian Gazette_ was much more extensive (affecting all mucous membranes in the body).  

The term "catarrh" is mentioned 728 times in all the digitized copies of the _Egyptian Gazette_. Of the 728 mentions, only four of those mentions were not in advertisements (nearly all of these mentions came from Peruna advertisements but around three came from another patent medicine). One was a sad story about a man suffering from catarrh who committed suicide (not, according to the article, because of the catarrh). The other three mentions remarked about notable personages suffering from catarrh. It seems like the meaning of the disease catarrh changed through the century. Although the term catarrh is uncommon in this region of the world today, when used, it essentially means the same thing it did during the time of the _Egyptian Gazette_.

Some additional material that I found is lists of diseases within advertisements. While Peruna concentrated on sickness, Allenburys’ appears to be a company that concentrated on supplements or fortifying food, almost like vitamins today. Allenburys’ advertised itself as a restorative medicine, but also as a preventative diet. The most common version of the advertisement was the one summarized as the “Strength and Stamina” advertisement. 

![Allenburys' Advertisement Distribution of Topics](IDS-2681-Analysis-Project-Image-Allenburys'-Content.png)

![Dr. William's Pink Pills Spreadsheet of Illnesses Mentioned](IDS-2681-Analysis-Project-Image-Dr.-William's-Pink-Pills-Content.png)

The last patent medicine considered in this research is Dr. William’s Pink Pills. The most common ailment the Pills claimed to cure was rheumatism followed by anemia, indigestion, and sciatica. As seen in the image above, it seems almost random which disease the advertisement claims to cure each time. 

I used variations on the following XPath queries to find the data. 
- `//div[matches(.,'peruna', 'i')][@type="advert"]/div`
- `//div[matches(.,'catarrh', 'i')][not(@type="advert")]/p`

These queries have problems because the unit `[not(@type="advert")]` is not always reliable. Sometimes a type is not used to define an advertisement. The other difficulty with this research topic is the lack of reliable information on historical illnesses. The reson I chose Peruna, Dr. William's Pink Pills, and Allenburys' is they are the most common medicinal advertisements. This topic has many ways to expand upon the small amount of research I completed. Future research could expand upon each disease mentioned in the advertisements. Another idea for future research would be to compare treatment methods of the diseases to modern treatments. This research hardly covered any of the topic. There is much more to discover within the topic of 1900s illnesses and their treatments.

## Works Cited

- Jones, C. Handfield. “Catarrh.” The British Medical Journal, vol. 2, no. 143, 1859, pp. 772–76. JSTOR, http://www.jstor.org/stable/25193777. Accessed 2 Dec. 2022.

- "What is Catarrh and How to Get Rid of It." Johnson & Johnson (Ireland) Limited. (2022) https://www.sudafed.co.uk/what-catarrh-and-how-get-rid-it. Accessed Dec. 2, 2022.

- “Catarrh.” Merriam-Webster.com Dictionary, Merriam-Webster, https://www.merriam-webster.com/dictionary/catarrh. Accessed 2 Dec. 2022.