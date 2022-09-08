---
title: Digital Egyptian Gazette Schema
linktitle: Schema
toc: true
type: docs
date: "2019-08-29"
draft: false
menu:
  resources:
    parent: Resources
    weight: 4

weight: 4
---
This page describes the schema used in the Digital Egyptian Gazette project, which lives [here](https://github.com/dig-eg-gaz/resources/blob/master/egSchema.odd) in [ODD (‘One Document Does it All’)](http://www.tei-c.org/Guidelines/Customization/odds.xml) format.

The schema expressed in relaxNG compact (made from .odd files using the [Roma tool](http://www.tei-c.org/Roma/) at [TEI-c.org.](http://www.tei-c.org/Roma/)) is [here](https://github.com/dig-eg-gaz/resources/blob/master/egSchema.rnc). It can be validated against by using the URL [https://raw.githubusercontent.com/dig-eg-gaz/resources/master/egSchema.rnc](https://raw.githubusercontent.com/dig-eg-gaz/resources/master/egSchema.rnc) in an XML editor.

In addition to the tags offered by the [TEI P5 guidelines](http://www.tei-c.org/release/doc/tei-p5-doc/en/html/index.html), the customized schema employs the following terms.

## `<div>` attributes

### Type
- nameplate: use for the first page of the paper only
- page: always use the `n=""` attribute
- item: the default and most generic `div` type
- section: a `div` containing other `div`s, typically of the `item` type.
- subsection: a `div` within a `section` itself containing other `div`s, typically of the `item` type. Use sparingly
- cable: a single wire report with a `<dateline>` and the name of the wireservice (typically Reuters or Havas)
- advert: any advertisement; templates are listed [here](https://dig-eg-gaz.github.io/advertisements)

### Feature
- weather: Daily Weather Report
- wire: Telegrams
- local: Local and General
- sport: Sport and Play
- social: Personal and Social
- comingEvents: Calendar of Coming Events
- passList: Passenger List
- visitList: Visitors' List
- letters: Letters to the Editor
- mattersMoment: Matters of Moment. Pith of the Press Comments.
- nativePress: Native Press Comments
- khedive: The Khedive
- esbekieh: Esbekieh Gardens
- army: Army and Navy / Army of Occupation / Egyptian Army
- shippingMovement: Shipping Movement
- steamerMovement: Steamer Movement
- navalNotes: Naval Notes
- mouvementMaritime: Mouvement Maritime
- londonLetter: Our London Letter
- parisLetter: Our Paris Letter
- prepaidAdvertisements: Cheap Prepaid advertisements
- bulletinBourse: Bulletin de la bulletin
- councilMinisters: Council of Ministers
- shareMarket: Egyptian Share Market
- notesPortSaid: Notes from Port Said
- notesSuez: Notes from Suez
- notesSuakin: Notes from Suakin
- notesKhartoum: Notes from Khartoum
- notesConstantinople: Notes from Constantinople
- notesCyprus: Notes from Cyprus
- notesSudan: Notes from the Sudan
- notesFayoum: Notes from Fayoum
- notesOther: Notes from other places in Egypt

### Status
Do not use any status as default--leave out the attribute altogether.

- verified: Complete and correct, verified by third editor.
- unverified: Has not been checked. 
- uncorrectedOCR: Div contains pasted OCR text that has not been corrected or formatted.
- irregularFormat: Div contains valid content, but formatting differs from standard.
- templateDefault: Div is identical to the template, and does not correspond to the content of the issue.
- empty: Div is empty, often because an editor deleted default template.
- incomplete: Div contains some but not all of the material it should.

## `<measure>` attributes

### Units
- tal: Talari
- cantar: qantar
- £: British Pounds Sterling
- fcs: francs
- sh: shillings
- LE: Egyptian pounds (livres égyptien)
- balles: bales of cotton
- ton: tonnes
- dC: degrees celsius
- mm: millimeters
- pt: piasters tarif
- min: minutes
- LE M: Egyptian pounds and millimes
- ard: ardeb
- $: US dollars
- sack: sacks

### Commodity
- currency

### Type
- indexNo: number corresponding to indexing system for newspaper features, especially paid advertisements

## Columns
- cols: Specifies the number of columns in a given section
- colSpan: Used to specifies the width of a div which spans multiple columns and cannot be accurately described using the cols and cb elements.