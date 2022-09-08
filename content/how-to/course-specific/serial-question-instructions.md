---
title: Serial question analysis instructions
linktitle: Serial question
toc: true
type: book
date: "2016-09-30"
draft: false
menu:
  course-specific:
    parent: Course specific
    weight: 2

weight: 2
---
Your final project is to consider a theme or question that recurs across many issues of the *Egyptian Gazette*.

Part of your work is to compose a serial question that makes sense and can be answered by the dataset. Explain this question (supplying, for instance, the xpath formula you will use), and explain how you extract the results. For guidance on queries, consult the [tutorial](/how-to/digitization/query-instructions).

To consult previous serial analysis projects, see this [directory](#directory-of-previous-analysis-projects).

## How do I format my serial analysis?

Write your file in [markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet), just as you did for the [blog post](/how-to/course-specific/blogging-instructions).

Use a header containing these lines. Supply the title, your name, and the date:

```
---
title: "YourTitle"
authors: [YourName]
date: YYYY-MM-DDD
categories: [analysis]
---
```

Name this file `index.md`.

## What about images?

Please produce data visualization(s) to accompany your analysis.

You may use a variety of tools:

- [Palladio](http://hdlab.stanford.edu/palladio/)
- [Google charts](https://developers.google.com/chart/)
- [Tableau](/how-to/digitization/visualization-instructions/)

## How do I show these visualizations in my markdown page?

The easiest thing to do is to take a screenshot and include the static image using markdown's code: `![image title](image-file-name.png)`.

If, however, you have produced an [interactive visualization](/how-to/digitization/visualization-instructions/) using Tableau or Google Charts, you need to do two things to embed data visualizations in your markdown github pages.

### 1. Host the visualization:

For **Tableau**:

Upload your workbook to Tableau Public's server. Use the "server" drop down menu and follow instructions. You will need to sign up for an online account, and you might have to save your dataset.

For **Google Charts**: 

Post your code as a [gist](https://gist.github.com/), then render it using a link from [githack](http://raw.githack.com/).

### 2. Embed the visualization:

For **Tableau**:

A complete version of embedding instructions is included in this [excellent tutorial](https://www.datavizforall.org/embed/tableau/). Briefly, you need to click the share icon at the bottom right hand side of your web-hosted visualization. Take the link that it offers and paste it into this code:

```xml
<iframe src="https://public.tableau.com/views/YOURURLHERE?:showVizHome=no&:embed=true" align="center" width="90%" height="500"></iframe>
```

(For the `YOURURLHERE` part, include everything to the right of `views/` and to the left of the question mark. Your line should look something like this: `<iframe src="https://public.tableau.com/views/MESAPresentation/Honorifics?:showVizHome=no&:embed=true" align="center" width="90%" height="500"></iframe>`.) Paste this code into your markdown file.

For **Google Charts**:

Place the following bit of code in a markdown file, and your visualization should appear: `<iframe src="your-githack-link" width="90%" height="400"/>`

## How do I submit my individual project?

Fork the [analysis](https://github.com/dig-eg-gaz/analysis) repository. Then, make a folder called named `19-analysis-yourSurname` and add it to this fork. Add your analysis text file (named `index.md`) to this folder, as well as your images. Make sure that you have no spaces in your file names--use dashes instead. Once your folder is complete, send a pull request. Do this at least twice: first you've finished a draft, and a second time once you've completed your analysis. It is fine to do it more often too, sending partial material or drafts. I will make comments, and you can revise them.

## How do we submit our group work?

One member of the group should add a folder named `19-analysis-yourGroupTopic` to their fork of the analysis repository. This folder should be structured the same as the individual project: an `index.md` file and image files. In the `author:` line of the markdown header, list all members of the group.

## Directory of Previous Analysis Projects

### IDS 2681 Fall 2019

Surname|Title
---|---
|**[An Accidental Analysis](/post/19-analysis-accidents)**
Crisafulli|[Emotions and Accidents](/post/19-analysis-chrisafulli)
Grant|[Polo in Egypt: An Attendance Analysis](/post/19-analysis-grant)
House|[The Geography of Accidents](/post/19-analysis-house)
Kamata|[Comparing Location and Speed to Analyze the Effectiveness of Communication](/post/19-analysis-kamata)
Nguyen|[Accidents Linguistics](/post/19-analysis-nguyen)
Walter|[Alexandria Fire Accidents](/post/19-analysis-walter)
|**[Medicine](/post/19-analysis-medicine)**
Dorsey|[Diseases and the Medical Schools/Hospitals History](/post/19-analysis-dorsey)
Heflin|[Tuberculosis and Medicine](/post/19-analysis-heflin)
Himmel|[Cholera](/post/19-analysis-cholera)
Naranjo|[The Plague](/post/19-analysis-naranjo)
Theophilopoulos|[Medical Terminology](/post/19-analysis-theophilopoulos)
|**[Sports](/post/19-analysis-sports)**
Faynberg|[Polo in Egypt: An Attendance Analysis](/post/19-analysis-faynberg)
Hesse|
Hayes|[Billiards Participants](/post/19-analysis-hayes)
Reynolds|[Home Field Advantage in Football](/post/19-analysis-reynolds)
Roche|[Horse Racing in 1907](/post/19-analysis-roche)
|**[Heat of the Sun](/post/19-analysis-sun)**
Hernandez|[Maximum and Minimum Temperature in Alexandria, Egypt(May 1906-April 1907)](/post/19-analysis-hernandez)
Monaco|[Maximum Heat of the Sun in Different Stations Across Alexandria [May 1906-April 1907]](/post/19-analysis-monaco)
Seguin|[Minimum Temperatures of Alexandria, Port Said, and Suez [1906-1907]](/post/19-analysis-seguin)
Smith|[Wind speeds in relation to the heat of the sun](/post/19-analysis-smith)
|**[Economic History of Stocks and Shares](/post/19-analysis-stocks)**
Chen|[The Mystery of Daira Sanieh](/post/19-analysis-chen)
Kim|[Egypt Stocks & Shares](/post/19-analysis-kim)
Kolby|
Ku|[Egypt’s Cotton Exports in the Early 1900s](/post/19-analysis-ku)
Mendez|[Gold Mining and the Gold Market:To What Extent does the Nile Valley Gold Company Reflect the Gold Market?](/post/19-analysis-mendez)
Piraino|
|**[Environment](/post/19-analysis-environment)**
Bryant|[The Cotton Worm in Egypt from 1905 to 1907](/post/19-analysis-bryant)
Grimaldo|[Mosquitoes in the Egyptian Gazette](/post/19-analysis-grimaldo)
Rivera|[Impact of Seasonal Change On Tourism and Hotel Stays](/post/19-analysis-rivera)
Simmers|[Cotton Production In Relation To Average Temperature in Alexandria](/post/19-analysis-simmers)
Thomas|[Humidity and its relation to cotton yields](/post/19-analysis-thomas)
---|---
Douglas|[Insurance vs Assurance](/post/19-analysis-douglas)

### IFS 2116 Spring 2018

Surname|Title
---|---
Arenas|[Attitudes towards Germany: Random, Situational, or Seasonal?](/post/18-analysis-arenas)
Beasley|[Temperatures in Assouan and Port Said](/post/18-analysis-beasley)
Bolger|[Polo in Cairo](/post/18-analysis-bolger)
Bridges|[Local and General Analysis](/post/18-analysis-bridges)
Brown|[Jobs in Cheap Prepaid Advertisements](/post/18-analysis-brown)
Cannon|[Reported Accidents, Incidents, Tragedies, and Disasters](/post/18-analysis-cannon)
Castro|[Theatre](/post/18-analysis-castro)
Chapple|[Hotels in Cairo](/post/18-analysis-chapple)
Clark|[The Egyptian education system in the early 1900s](/post/18-analysis-clark)
DeGroat|[Rainfall](/post/18-analysis-degroat)
D'Onofrio|[Robberies in Alexandria](/post/18-analysis-donofrio)
Ebert|[Egyptian Export Companies](/post/18-analysis-ebert)
Ell|[Wedding and Funeral Flowers](/post/18-analysis-ell)
Frady|[Marriage, Weddings and Divorce](/post/18-analysis-frady)
Fitzpatrick|[The Fascination with Death](/post/18-analysis-fitzpatrick)
Hutson|[The Big Four Theatres](/post/18-analysis-hutson)
Jones|[Humidity in Alexandria](/post/18-analysis-jones)
Majonica|[Letters to the Editor 1906](/post/18-analysis-majonica)
Mason|[Most Popular Sports](/post/18-analysis-mason)
Medina|[The Plague in Egypt](/post/18-analysis-medina)
Metallo|[Stocks and Shares](/post/18-analysis-metallo)
Meyer|[Fires](/post/18-analysis-meyer)
Northcutt|[Anti-Semitism in Egypt and Surrounding Countries](/post/18-analysis-northcutt)
Pierre|[Communication is the way](/post/18-analysis-pierre)
Porter|[Golf in Egypt in the early 20th century](/post/18-analysis-porter)
Pregasen|[Lord Cromer in the Egyptian Gazette](/post/18-analysis-pregasen)
Pustam|[Wedding Fashion Trends 1905-1906](/post/18-analysis-pustam)
Richardson|[Children in Alexandria](/post/18-analysis-richardson)
Squires|[Impact from Climate in Alexandria](/post/18-analysis-squires)
Wallace|[Shipping in Colonial Egypt](/post/18-analysis-wallace)

### IFS 2116 Spring 2017

Surname|Title
---|---
Acosta|[Patent Pills](/post/17-analysis-acosta)
Ali|[Egypt's Grandest Stage](/post/17-analysis-ali)
Anderson|[Tarif d’Exportation](/post/17-analysis-anderson)
Baenen|[Seasons of Sport](/post/17-analysis-baenen)
Barrett|[Donkeys](/post/17-analysis-barrett)
Baxter|[New York Excursions](/post/17-analysis-baxter)
Bolton|[Vade Mecum for the Homeward Bound](/post/17-analysis-bolton)
Boucher|[Bond Price Analysis](/post/17-analysis-boucher)
Chacon|[Murder locations](/post/17-analysis-chacon)
Cwikla|[Analyzing Archaeology](/post/17-analysis-cwikla)
Doring|[The Ground War in China](/post/17-analysis-doring)
Fajardo|[Bubonic Plague](/post/17-analysis-fajardo)
Ferguson|[20th Century Mosquito Control Efforts in Egypt](/post/17-analysis-ferguson)
Fitzpatrick|[Murder Reports](/post/17-analysis-fitzpatrick)
Flick|[Funerals](/post/17-analysis-flick)
Frazier|[Desert weather](/post/17-analysis-frazier)
Fricano|[Cotton trade](/post/17-analysis-fricano)
Greco|[Coal in Early 1900s Alexandria](/post/17-analysis-greco)
Hammermaster|[Changes in the Murder Rate in Alexandria](/post/17-analysis-hammermaster)
Hayden|[Sailboat Racing](/post/17-analysis-hayden)
Hensley|[Insurance](/post/17-analysis-hensley)
Horton|[Hospitality through the eyes of the Egyptian Gazette](/post/17-analysis-horton)
Johnson|[The Domino Effect: The Impact of Strikes, 1905-1906](/post/17-analysis-johnson)
Martinez|[Land Bank Stock Prices](/post/17-analysis-martinez)
Meixner|[Patterns and Trends with Weddings](/post/17-analysis-meixner)
Migdalski|[Plague in Egypt, 1905-1906](/post/17-analysis-migdalski)
Morales|[The Plague and the roles hospitals played](/post/17-analysis-morales)
Muniz|[Russian Revolution](/post/17-analysis-muniz)
Nuñez|[Russian Revolution](/post/17-analysis-muniz)
Ng|[Front Page Advertisements](/post/17-analysis-ng)
Ortiz|[Anarchism in Colonial Egypt](/post/17-analysis-ortiz)
Pearce|[Turn of the Century Exchange Rates](/post/17-analysis-pearce)
Petersen|[Gum in Egypt](/post/17-analysis-petersen)
Rodriguez|[Murder in Alexandria](/post/17-analysis-rodriguez)
Sepulveda|[1905 County Championship](/post/17-analysis-sepulveda)
Story|[Climate Change in Alexandria](/post/17-analysis-story)
Ukah|[Aspects of Insurance](/post/17-analysis-ukah)
Vaverek|[Making Sense of the Daily Weather Report](/post/17-analysis-vaverek)

### IFS 2116 Fall 2016

Surname|Title
---|---
Amorello|[Letters to the Editor in the 1905 Egyptian Gazette](/post/16-analysis-amorello)
Barbosa|[Murder](/post/16-analysis-barbosa)|archive
Barrett|[Sports](/post/16-analysis-barrett)
Black|[Investigating the Calendar of the Week](/post/16-analysis-black)
Caliendo|[20th Century Smoking Culture](/post/16-analysis-caliendo)
Cooper|[Who is the Fastest Horse in Alexandria?](/post/16-analysis-cooper)
Corzo|[Silent Killer](/post/16-analysis-corzo)
Crawford|[Capital Market Integration](/post/16-analysis-crawford)
Crespo|[Nile River](/post/16-analysis-crespo)
Curcio|[Medical Miracles](/post/16-analysis-curcio)
Cyr|[Bubonic Plague In Egypt, 1905](/post/16-analysis-cyr)
Esteve|[The Uses of Counting](/post/16-analysis-esteve)
Eugenio|[The Bubonic Plague](/post/16-analysis-eugenio)
Evanoff|[Advertising in Alexandria Egypt 1905](/post/16-analysis-evanoff)
Fling|[The Egyptian Gazette’s Fires of 1905](/post/16-analysis-fling)
Frederick|[The African Pygmies](/post/16-analysis-frederick)
Gressgott|[Anti-Semitism](/post/16-analysis-gressgott)
Grieco|[Fluctuation in Egyptian Cotton Exports Throughout the Year](/post/16-analysis-grieco)
Heyward|[How Much Coal was Imported Into Egypt in 1905?](/post/16-analysis-heyward)
Hofmeister|[Changes Over the Year](/post/16-analysis-hofmeister)
Lappin|[Cultural Significance of Events in Alexandria](/post/16-analysis-lappin)
Ouelette|[Analysis](/post/16-analysis-ouelette)
Ragland|[The Exploration of Musicians in Alexandria](/post/16-analysis-ragland)
Rymer|[Egyptian Entertainment: Weekend activities of the everyday Egyptian in 1905](/post/16-analysis-finalproject-rymer.pdf)
Sain|[Tracking Stray and Ownerless Dogs](/post/16-analysis-sain)
Stefonek|[Fleet Tracking](/post/16-analysis-stefonek)
Summa|[A Serial Analysis of St. Petersburg, London, and Paris Through the Lens of the Egyptian Gazette](/post/16-analysis-summa)
Taylor|[Expeditions in 1905](/post/16-analysis-taylor)
Thompson|[The Deaths of Alexandrian Citizens in 1905](/post/16-analysis-thompson)
Vazquez|[How did the Cattle Plague affect populations during the year of 1905?](/post/16-analysis-vazquez)
Vincent|[Tragic Events in 1905](/post/16-analysis-vincent)
White|[Counting Countries, Counting Cities](/post/16-analysis-white)
Wills|[Global Diplomatic Influence on Egypt](/post/16-analysis-wills)

