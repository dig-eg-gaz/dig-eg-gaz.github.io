---
title: Polishing TEI instructions
linktitle: Polished TEI
toc: true
type: book
date: "2019-10-01"
draft: false
menu:
  digitization:
    parent: Digitization
    weight: 70

weight: 70
---

## Objective
This lesson explains how to polish your TEI-XML file so that it is ready to be added to the master content repository.

## 1. Get the page hierarchy right

The best way to get a quick idea of your file's structure is to look at the Outline in Oxyge. At the highest level, your document should consist of six (or eight) parallel page `<div>`s:

![page-div-outline](page-div-outline.png)

All other `<div>`s should be _inside_ the page `<div>` in which they appear. If you do not have everything inside pages, your outline will look messy:

![page-div-outline-messy](page-div-outline-messy.png)

The solution is to drag everything into its proper page. 

Another problem that arises is failing to close divs or pages. You'll know you have this problem if the end of your file looks like this:

![unclosed-divs](unclosed-divs.png)

## 2. Get the breaks right

There are three types of "breaks" in the digital _Egyptian Gazette_. All are indicated using single tags, rather than pairs: unlike paragraph tags, for example, which must open (`<p>`) and close (`</p>`), break tags come alone. They include a "slash" just before the closing bracket to show that they have no partner: `<lb/>`. 

Two of the break tags are quite straightforward to work with:

### a. Line breaks

You will have little need for line breaks, which are coded `<lb/>`. For the most part, line breaks are indicated with paragraph tags. Sometimes, however (in adverts, for instance), you may find it useful or necessary to use a `<lb/>` instead of `<p></p>`.

### b. Page breaks

Page breaks (`<pb n="?"/>`) are currently used in the digital _Egyptian Gazette_, but they are redundant, because every page is contained in `<div type="page" n="?"> </div>` tags. In both cases, the `n="?"` attribute records the page number.

Please use both divs and breaks to indicate pages. TEI's rules for periodicals are still in development, and we want our resource to be flexible to more than one approach. Note that the page break tag comes _before_ the page `<div>` itself; the arrangement outlined in the first page hierarchy image above is correct.

## 3. Column breaks

Column breaks can be hard to work out, not least because they are not well implemented in the TEI specification. In this project, we use three different tags to describe the columns:

### a. `<cb n="?"/>`
This tag indicates the start of a new column. Use it at the beginning of every page, and again each time the text stops at the bottom of the page and jumps to the top of another column. Use the `n=` attribute to indicate which column is beginning. 

This is straightforward on a typical page 3, which contains six even-sized columns running from the top to the bottom of the page. 

![cols-example-6-cbs-p-3](cols-example-6-cbs-p-3.png)

Do not make each column into its own `<div>`. Column breaks often coincide with the start of a new `<div>`, but they have a distinct role. They indicate the layout of the paper, not its content. `<div>`, on the other hand, is used to encode articles and sections of the paper with their own headline and content. A `<cb/>` can even be dropped in the middle of a paragraph, as we see with the column break at the start of column 5 in the image above.

### b. `<cols n="?"/>` 
This tag indicates how many evenly-sized columns the page is divided into. Use it only when the width of columns change. Below the nameplate on page 1, for example, we use a `<cols n="3"/>` tag to show that the page is divided into three equal columns. We insert this tag before we show the start of the first column using `<cb n="1"/>`.

Page 3 is usually divided into six equal columns. We can indicate this using `<cols n="6"/>`. Again, this tag comes before the first column break (as indicated in the image above).

Things are more complicated on page 2, which often contains a mix of single- and double-width columns. Remember that single-width columns are indicated with `<cols n="6"/>`, because the page can contain six of them. Double-width colums are indicated with `<cols n="3"/>`, because the page can contain only three of them. The rare triple-width column would be marked with `<cols n="2"/>`.

Here is an example of a page 2, with its layout blocked in colored columns:

![cols-example-p-2-layout](cols-example-p-2-layout.png)

The page starts with a double-width column (A), which splits into two single-width columns (A & B) partway down. The middle of the page contains another double-width column ( C ) that splits into single-width columns (C & D). The right-hand side of the page contains two full-length single-width columns (E & F).

We encode the columns on this page like this:

![cols-example-p-2-layout-xml](cols-example-p-2-layout-xml.png)

### c. `<colSpan n="?"/>` 
You will rarely need to use this tag. It is only used for items that are wider than a single column located where the page cannot be divided into even-sized columns using `<cols/>`.

For example, the "Nile Gauge Reading" item at the bottom of this page should be preceded by a `<colSpan n="4"/)` tag.

![cols-example-colspan-4](cols-example-colspan-4.png)