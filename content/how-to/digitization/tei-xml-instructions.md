---
title: TEI-XML instructions
linktitle: TEI-XML
toc: true
type: book
date: "2016-09-05T00:00:00+01:00"
draft: false
menu:
  digitization:
    parent: Digitization
    weight: 20

weight: 20
---

## Objective
These instructions guide you in transforming your plain text page files into a marked-up xml document that conforms to the standards of [TEI](http://www.tei-c.org) (the Text Encoding Initiative).

## 1. Set up your XML editor
Download the full-function Oxygen XML Editor, which offers a [free 30-day trial](http://www.oxygenxml.com/xml_editor/register.html). After 30 days, you might find [ways](https://10minutemail.com/) to renew your trial access, or simply purchase Oxygen using their [academic and educational discount](http://oxygenxml.com/academic/)).

## 2. Create an xml file
Copy and paste [this template](https://raw.githubusercontent.com/dig-eg-gaz/boilerplates/master/empty-issue.xml) into a new document. **Important**: the new document will have `<?xml version="1.0" encoding="UTF-8"?>` as its first line, and it's also the first line of the template; delete one of them, otherwise your document will be ill-formed. Name this document using the date of the issue and an xml extension (YYYY-MM-DD.xml). (This document will eventually contain all of the pages of the issue, so it is not necessary to add the page number to the document name.) Save this document on your hard drive.

## 3. Fill in the header
Enter your name into the template (under `<editor>`), today's date (under `<edition>`, in text and numeric formats), and the issue date (under `<bibl>`, in text and numeric formats). (Currently, these areas have entries in the comment format (`<!-- -->`)--replace these with your text). Save your file.

## 4. Copy and paste templated material
In your xml document, the text of your issue itself (as opposed to just the header) starts like this:

![page-1-example](/img/page-1-example.png)

The "nameplate" `<div>` that you see here represents the banner at the top of page 1, which contains the title of the newspaper, the number, date, number of pages, and price, and is flanked by two advertisements: 

![nameplate](/img/nameplate.png)

You will need to update your xml file to reflect the content of your own issue. First, you need to look in the [advertisements directory](/issues/advertisements) to find templates that correspond to the ads that appear in your issue. Following the detailed indications [here](/how-to/digitization/templating-instructions/), copy the xml text of templates you need.

You must paste this text into the correct spot in the nameplate of your xml document. The two ads flanking the title take the form of `<cell>`s that go in the first `<row>` of the nameplate. The second `<row>` of the nameplate lists the number, date, and number of pages of the issue. Update this information.

![nameplate-2nd-row](/img/nameplate-2nd-row.png)

If you switch to author mode (choose it from the text-grid-author buttons near the bottom of your screen), the whole nameplate should look something like this:

![author-mode-nameplate](/img/author-mode-nameplate.png)

Now switch back to text mode and proceed to work on the rest of the page. Find the text of the first ad in the first column after the nameplate, and paste it after the `<cb n="1"/>` tag in the advertising section division. Proceed inserting ads all the way to the end of the third column.

## 5. Make sure that your document is well-formed
At the top right hand corner of your editing window in Oxygen, there is a square that will be either red or green. If it's green, your document is well-formed, which means that it conforms to TEI XML standards and will be searchable and useable. If it's red, the file contains errors that you must fix before you submit it. The errors appear as red lines on the right hand scrolling column. Click on a line to see the error described at the bottom of your editing screen.

One common error that prevents a well-formed document:

- doubled `<?xml version="1.0" encoding="UTF-8"?>` lines at the opening of the xml document.

## Resources
- “[A Gentle Introduction to XML](http://www.tei-c.org/release/doc/tei-p5-doc/en/html/SG.html),” TEI Consortium.
