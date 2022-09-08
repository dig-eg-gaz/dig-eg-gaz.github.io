---
title: "Accidents Linguistics"
authors: [PhuongNguyen]
date: 2019-12-03
categories: [analysis]
---

One aspect that can be used to describe accidents is the linguistic descriptions of the accidents within the Egyptian Gazette. The most descriptive terms come prior to the word “accident,” so the best start to using XML and querying was to search for “accident” and restrict it to headers with “head.” This resulted in 145 items. This was then copied and pasted into atom. Atom was used to cut the extra text down to the words in between the <head> and </head> in the Description lines by searching the buffer for the System ID: line, Match:, Start line, and Length line and replacing them all with empty space. The only lines saved were those containing “accident” or “accidents.” I did not take into consideration the possibility of “accident” being misspelled in a way that Atom couldn’t recognize. Articles like 14 “the”s were replaced. 12 “a”s were erased by using \sa\s (blank space, a, blank space) so as not to replace a’s within words. They were replaced with empty space. All periods were erased by turning off regex and were replaced with empty space. I found XML language stuck in the buffer somehow (Match:) by using <\w+. I was unsure of how to do a full erasure from < to > and end header, but there were only three lines, so I simply erased them.  One was “Description.” All were replaced with empty space.  I then used Atom to find \r\n\r\n to replace the long empty spaces with \n.

One problem I approached were the spaces in front of lines that I had caused from replacing A’s with a space. I didn’t know of a way to fix this automatically without redoing all of the previous work, so I replaced them by hand with \s. Double spaces were replaced with one space too.

After saving this file, I opened a new file and copied over same saved data. I deleted all “to”s with /sto/s and all the “at”s with \sat\s.

I erased all the “accident” and “accidents” because I only wanted the descriptions in the visual representation since the subject was the descriptions rather than the word accident itself. I deleted leftover spaces individually.

After inserting the list into wordcloud.com, I encountered another problem: the same words showed up more than once if they were fully capitalized or fully in lowercase or even had only the first letter capitalized.
I then used the shortcut using the Shift key and F3 which put the entire list in all caps.

Another problem was encountered: some ”common words” are actually connected to the primary words, which is fine to just look and add back to.

Another problem: some of these words have the same meaning, i.e. drowning and bathing, motor and car, car and tramway probably refer to the same things.

The data was put into an excel spreadsheet and connected that to tableau by.

I deleted the “ on “implacable inside tableau to keep ABC order.

`accident\w?\w?\w?\w?\w?\w?\w?\w?\w?\w?\w?\w?\w?\w?\w?\w?\w?\w?\w?\w?\w?\w?`

Using this long stretch of text, I erased words that included the word “accident” such as the word itself and “accidents”, “accidentally”, etc. (under “accident p”, xml was for paragraphs (and heads) containing the word “accident.”

“…” was erased. One trouble I don’t know how to solve was capturing the whole paragraph instead of just parts of it. I think this should suffice as the best option, since trying to capture the entire paragraphs in other ways lead to only obtaining lines that didn’t have the word “accident” at all. .
T
he next step is to have the words counted and categorized and graphed, and top words compared to the simple list of words previously.

“one” and “two” and the number “0” are excluded from the top word frequency list.

Replaced \r\n with empty space.

Replaced empty spaces with a single space.

 “- “ erased because it is mostly signaling words that are split.

There are words that are in the headlines that correspond to the whole paragraph, but aren’t necessarily top twenty-five, but there are scarcely any words that were frequent in the paragraph that are frequent for the headlines. Out of the top twenty-five reoccurring words for each, only four have corresponded. Top 25 happen to be where the frequency of words for headlines is more than one. Since paragraphs contained higher counts of words like "train" and "railway", but headlines contained higher counts of  "fatal", "railway", "motor", and "tram", one can see that the word "fatal" is a signal for readers that there is an important accident. This also shows that there is a high probability that most reoccurring accidents are firstly train accidents and secondly motor accidents.

Having the top four words in common be "cairo", "injured", "railway", and "train" show again that train accidents occur the most and are presented most frequently, as well as having a strong basis in Cairo. "Injured" is a common word used for both show and description- a signal for readers that a person was affected but also a common description for readers to catch onto.

According to "Reported Accidents, Incidents, Tragedies, and Disasters", accidents can be categorized under "vehicles" or general headlines (Cannon). The author discussed that accidents are also described using different words such as "incidents", "tragedies", and "disasters." This shows that there can be many missing descriptions or occurrences that I missed due to language variations.  

## Data Visualization:

<iframe src="https://public.tableau.com/views/CombinedAccidentsBarGraph/Sheet1?:showVizHome=no&:embed=true" align="center" width="90%" height="500"></iframe>

<iframe src="https://public.tableau.com/views/CombinedAccidentsBarGraph/Sheet1?:display_count=y&publish=yes&:origin=viz_share_link" align="center" width="90%" height="500"></iframe>

## Sources:
- Cannon, Jonathan. “[Reported Accidents, Incidents, Tragedies, and Disasters](dig-eg-gaz.github.io/post/18-analysis-cannon/).” Digital Egyptian Gazette, Will Hanley, 16 Apr. 2018.
