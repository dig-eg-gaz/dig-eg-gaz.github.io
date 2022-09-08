---
title: Features
linktitle: Features
toc: true
type: book
date: "2016-09-30"
draft: false
menu:
  issues:
    parent: Issues
    weight: 4

weight: 4
---
The *Egyptian Gazette* contains a large number of recurring elements. Some of this material is captured in [templates](/contents/templates/), and others are [advertisements](/contents/advertisements). This pages lists recurring free-text elements, which this project identifies using the `feature` attribute. This visualization shows the frequency with which features are distributed:

<iframe src="https://public.tableau.com/views/EgyptianGazettefeaturesdistribution/Commonfeaturesday?:showVizHome=no&:embed=true" align="center" width="90%" height="500"></iframe>

Recurring Element Name(s)|Feature attribute|Usual Page(s)|Frequency|Notes
---|---|---|---|---
**[Advertisements](/contents/advertisements/)** |none--identified using `xml:id` attribute|1, 2|daily|Use [templates](/contents/advertisements/)
**[Daily Weather Report](/contents/templates/#daily-weather-report)** |"weather"|2|daily|[tempate](https://github.com/dig-eg-gaz/boilerplates/blob/master/boilerplates-text/daily-weather-report.xml) [alternate tempate](https://github.com/dig-eg-gaz/boilerplates/blob/master/boilerplates-text/daily-weather-report-02.xml)
**Birth / Death / Marriage** |"birthDeathMarriage"|2||Single-line paid announcements
**Telegrams / Wire Reports / To-day's telegrams** (international news)|"wire"|3, 4, 5|daily|Sometimes there is no headline for this section. Treat cables as individual divs (`type="cable"`), each with its own `<dateline>` and `<title>`. This section is sometimes spread over two pages; when this is the case, you can use the `next` and `prev` attributes.
**Local and General** |"local"|3|daily|Treat individual paragraphs as individual divs (`type="item"`), each with its own `<head>`.
**Sport and Play** |"sport"|3, 5|daily?|Treat contents as items, each with own headline.
**Personal and Social** |"social"|3|daily?|Treat contents as paragraphs
**The Khedive** |"khedive"|3|daily?|
**Council of Ministers** |"councilMinisters"|3||
**Letters to the Editor** |"letters"|3||Treat each letter as an item, with `<byline>` and `<dateline>`
**Native Press Comments** |"nativePress"|3||
**Band Performance / Esbekieh Gardens** |"bandPerformance"|3||Lists concert program. Format concert program as a `list`
**Obituary** |"obituary"|3||Article on life of a resident of Egypt. Do not use for one-line obituary items in the Telegram section.
**Passenger List** |"passList"|3,4,5,6,7||Treat arrivals and departures as items.
**Steamer Movements** |"steamerMovements"|3|Almost daily.|Arrivals and departures of passenger ships. Treat contents as paragraphs.
**Shipping Movements** and **Mouvement Maritime**  |"shippingMovements"|4,6|Almost daily. |Arrivals and departures of cargo ships. French-language Mouvement Maritime runs to October 1905; English-language Shipping Movements begins November 1905; format as paragraphs.
**Délégation Municipale / Questions Municipales / Municipality** |"municipality"|3,4,6||
**Army and Navy / Army of Occupation / Egyptian Army / Naval Notes** |"army"|3,4,5,7||Often contain a `<dateline>`.
**[Calendar of Coming Events](/contents/templates/#calendar-of-coming-events)** |"comingEvents"|5|daily|see [template](https://github.com/dig-eg-gaz/boilerplates/blob/master/boilerplates-text/calendar-of-coming-events.xml) for format
**[Cheap Prepaid Advertisements](/contents/templates/#cheap-prepaid-advertisements)** |"prepaidAdvertisements"|2,5,7||Also listed as "Cheap Advertisements." Section template [here](/contents/templates/#cheap-prepaid-advertisements). Treat each advertisement as an item.
**Chronique Theatrale / Abbas Helmy Theatre / Alhambra Theatre / Zizinia Theatre / etc.** |"theatre"|3,4||Coverage of theatre performances
**Visitors' List** |"visitList"|3,5||Treat each hotel as an item.
**Matters of Moment / Pith of the Press Comments / Home Papers** |"homePapers"|5||Make into a section and divide contents into items.
**Legal Notes / Chronique Judiciare** |"legal"|3,4,6||French language
**Our London Letter** |"londonLetter"|7||
**Our Paris Letter** |"parisLetter"|7||
**Egyptological Notes** |"egyptological"|||
**Egyptian Share Market / Money and Share Market** |"shareMarket"|3,5|Usually Thursday|Section containing items (Egyptians, Mining, Consols, Rails, etc.) with own heads; often closes with a table. Name changes from Egyptian Share Market to Money and Share Market in February 1906.
**The Cotton Market** |"cottonMarket"|4||Kearsley and Cunningham’s Weekly Report
**Chronique Financiere** |"chroniqueFinanciere"|3,4|Usually Saturday|French language. Includes dateline.
**Circulaire H. de Vries et Boutigny. Notes et Critiques**  |"circulaire"|3,4||French language
**Bulletin de la Bourse**  |"bulletinBourse"|3,4,6||French language
**[Export Manifests](/contents/templates/#export-manifests)** |"exportManifests"|4,6,8||Use OCR and break each line into its own `<p>`.
**Notice / AVIS**  |"notice"|4,5,6,7||Annoucements of tenders and other business. Typically also feature the company or government (often the Alexandria Municipality) in the headline. AVIS is French language version, which is most common.

## "Notes from" section:
These notes typically appear on page 3. They are sourced to "Our Own Correspondent". Treat individual stories as `<div type="item">`, each with its own `<head>`. It is not always clear how many stories belong to the section.

Place|feature|Notes
---|---|---
Constantinople|"notesConstantinople"|also appears as Constantinople Notes
Port Said|"notesPortSaid"|
Suez|"notesSuez"
Fayoum|"notesFayoum"|also appears as Fayoum Notes
Cyprus|"notesCyprus"
The Sudan|"notesSudan"
Suakin|"notesSuakin"
Khartoum|"notesKhartoum"
Assiout|"notesAssiout"
Luxor|"notesLuxor"|also appears as Luxor Notes
Other|"notesOther"|Notes from Akhmin, Keneh, Kafr Zayat, Minet el Gamh, Wadi Medani, and other places in Egypt
