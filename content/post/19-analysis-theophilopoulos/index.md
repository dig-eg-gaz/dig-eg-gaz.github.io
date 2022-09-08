---
title: "Medical Terminology as a means of analysis for the progression of medicine in Egypt and the British Empire"
summary: "An analysis of the progression of miracle pill advertisement throughout 1905, 1906, and 1907 as a means to make inferences about the overall progression of medicine and marketing of medicines"
authors: [TryfonGerasimosTheophilopoulos]
tags: ["medicine"]
categories: [analysis]
date: 2019-12-10
---
## Introduction

In 1905, the world found itself in quite the predicament regarding medicine due to the relatively unknown cause and actual pathophysiological processes surrounding infection and contamination of a pathogen. Egypt and Alexandria in particular were still under British rule, as can be seen through the Egyptian Gazette, which is a primarily English containing newspaper marketed towards the British in the surrounding Egyptian areas as well as those who dealt with these individuals on a primary basis. In conclusion, this newspaper was made for the rich imperialists in control. Because of this, many different European and British influences can be seen within the Egyptian Gazette, one of which being certain medically affiliated advertisements. Two advertisements which caught my eye in particular were ones advertising Dr. William’s Pink Pills as well as Doan’s Kidney Pills.

![A Painful Portrait 1905-01-04](https://i.imgur.com/klxKSl2.png )

These pills were marketed as miracle pills that would be able to cure essentially any ailment that one encountered, including but not limited to kidney disease, heart palpitations, anxiety, stress, weakness, pain, backache, anaemia, clinical depression, poor appetite, and even cancer at one point. The funny part about the absurdness of the entire sales pitch?- they consisted of only iron oxide and magnesium sulfate. When looking into [a study](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5337769/ ) conducted by Reyhaneh Kheiri, et al., they found that iron oxide had no real positive effect on the body, and iron levels only slightly increased depending on the dose between 1-6 hours following consumption. 12 hours following consumption, no iron level change could be observed. Magnesium sulfate, on the other hand, does have some health benefits such as prevent low magnesium blood levels as well as seizures in women. It is *almost* unexpected that this compound also fails to treat any of the illnesses and conditions that these miracle pills claim to cure.

So what’s the catch? The simple answer is that these pills are entirely based on placebo and were such a large success due to the overall failure to understand medicine and pathology as we do today in modern medicine as well as the clever marketing that has been implemented not only in Egypt, but also worldwide during the selling of these pills. My analysis project deals primarily with the medical terminology which was employed in order to successfully market these “miracle pills”

To begin my analysis, I first had to find suitable advertisements that I would be able to use for this nature of a project. My main issue that I encountered was that most of the time, advertisements remain the same or only change once or twice throughout their lifetime in the Egyptian Gazette. This severely limited the advertisements that I would be able to use for this project, as I had to find more dynamic ones which were constantly changing on a daily or even monthly basis depending on the prevalence and frequency of them in the newspaper. I finally cut down all of the candidates I was originally looking at down to two: Dr. William’s Pink Pills & Doan’s Kidney Pills.

These advertisements seemed to be very different from other advertisements within the Egyptian Gazette in a couple different senses which made them perfect candidates for this embarkment. The main reason was because these advertisements often did not find themselves coming up within the main advertisement sections at all. The places that I found these advertisements were within actual bodies of text where stories and other items would be found. This meant that instead of being a reoccurring identical template, it changed constantly. In addition, because of this constant dynamic aspect that the advertisements had, they were often formatted in the form of a testimonial to make it seem less like a product being sold and more like an actual account from a civilian just like one who may be reading the newspaper, increasing their overall authenticity to the reader. In the end, this entire con is just a marketing scheme to make money, and it appears that these antics worked for a reason I will expand on when showing the data.

## Procedural Method for Obtaining Results

Firstly, due to the nature of these advertisements not actually being put into a advertisement div, I had to form my Xpath Query slightly differently so that it would find the instances of the title of the pills. I also was required to keep the Xpath Query fairly basic as narrowing it down in various ways resulted in not flagging positives as it should have been. For example, there was no template for these advertisements due to the fact that, once again, they were constantly changing throughout the Egyptian Gazette. The two queries that I used to create a database were the following:

//div/div/p[contains(., 'Pink Pills’)]

//div/div/p[contains(., ‘Doan’s Kidney Pills’)]

After moving all of the div’s into a plaintext file, I separated them by year and began looking for patterns and certain terminology that I deemed important and observed repeating throughout. I then took specific words that I found important and created a database of the occurrences that they came up in the advertisements. I also counted the number of each advertisement for each year and then created a ratio of instances of word : instances of the advertisement that year. That created a fraction of the average number of times a specific word came up in one advertisement, allowing me to properly compare between years. I then plotted this data using Tableau and came up with the following:

### Dr. William's Pink Pills:
<iframe src="https://public.tableau.com/views/Book1_15758293045230/Sheet1?:display_count=y&:origin=viz_share_link?:showVizHome=no&:embed=true" align="center" width="90%" height="500"></iframe>

&nbsp;

&nbsp;

&nbsp;

### Doan's Kidney Pills
<iframe src="https://public.tableau.com/views/Book1s_15758318890720/Sheet1?:display_count=y&:origin=viz_share_link?:showVizHome=no&:embed=true" align="center" width="90%" height="500"></iframe>

## Data Analysis

From this data, I was able to learn and infer a couple of different things. The first thing that stood out to me was the amount of times the advertisements for these “miracle pills” would come up throughout the Egyptian Gazette. For example, when looking at instances of Dr. William’s Pink Pills, in 1905 there were only 16 occurrences of the advertisement. In 1906, that number increased slightly to 19 instances. Then, in 1907, the number skyrocketed to 45 different instances of that advertisement throughout the year in the Egyptian Gazette. When looking Doan’s Kidney Pills, a similar jump can be observed in the Egyptian Gazette. In 1905, 11 instances were recorded, in 1906 12 instances were recorded, and in 1907 the number shot through the roof. This clearly goes to show that the success surrounding these pills was flourishing as much more money was able to be put towards advertising following what I believe was a good year or two of selling their product. I also believe that this is due to this relatively new method of advertising which implemented personal testimonials to sell the product.

Other patterns that I observed from this data was regarding exactly why many of these terms decreased in frequency over the three year time span. I believe after looking at the data and taking a detailed look into what types of treatments that the pills were offering that as medicine became slightly more advanced over this time period, these advertisements began to vouch for treating less and less serious ailments. They instead appear to move towards more general symptoms, the primary one being pain. These advertisements saw an increase in the prevalence of “pain” as pain can be associated with various illnesses, allowing them to generalize to more diseases without distinctly claiming to cure one or the other. As actual treatments for certain illnesses became available, these “miracle pills” began to advertise less towards specific ones and more for general symptoms.

Another example of this move towards a better understanding of modern medicine can be seen in the word “blood”. I observed a decrease in the word blood within both advertisements, primarily because medicine was becoming more advanced as actual understanding of the body and pathogens slightly deepened. It was a common misconception that many ailments were caused by an impurity in the blood, and that a way to get new blood was a way to prevent further illnesses. These pills claimed to give “new blood” to the user, although this logic is clearly flawed by today’s understanding. As the understanding of pathology increased during this time period, we can also see a decrease in the word “blood” coming up in the newspaper, leading me to believe that this assumption of blood impurities became less prevalent as other more accurate explanations for illnesses arose.
