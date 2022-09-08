---
title: Content markup instructions
linktitle: Content markup
toc: true
type: book
date: "2019-09-09"
draft: false
menu:
  digitization:
    parent: Digitization
    weight: 60

weight: 60
---

## Objective
This lesson explains how to convert the raw, basic XML text you produced through OCR into useable TEI-XML material.

## 1. Fix the basic structural tags
 Now correct and add basic structural tags of three types:

-  `<div type="item">`, which you can use for articles, items, or any division of the page that makes sense to you,
- `<head>`, which indicates a headline (the headline must be the first element in the item),
- `<p>`, which indicates a paragraph.

Oxygen offers many shortcuts to make this work go faster. Highlight the text you wish to wrap, then hit `command-E`. You will be offered a menu of tags. Choose the one you want. If you want to add more tags of the same type, hit `command-slash`.

Once you add these tags to your page, you might have a valid document (and thus a green box in Oxygen). But these common errors will probably also have to be addressed:

- **&**: the ampersand is represented as `&amp;` in xml. `&` alone will create an error.
- **>** or **<**: the OCR process produces stray angle brackets. The editor thinks these are part of a xml tag, and it causes an error.
- anything else not in a `<div>`, and not in a `<p>` or a `<head>`.

## 2. Add feature attributes
There are many recurring sections that show up issue after issue: local news, international news, sports, and many more. These should be marked `<div type="section">` rather than `<div type="item">`. It is important to mark these using the feature attribute, so that we can find them in XPath searches. The complete list of features is [here](/issues/features/). To add an feature attribute, place it within the `<div>` tag, after the `type="section"` attribute, thus: `<div type="section" feature="local">`. If you type `feature` inside the tag, Oxygen should offer you an autocomplete menu of features.

## 3. Add more complex structural tags
There are more tags that you can add:

- If the article or item is in French, add the attribute `xml:lang="fr"` to the `<div>` tag.
- **`<cb/>`** for column breaks. Be sure to put this tag at the *beginning* of the column. Add the number of the column, as well, thus: `<cb n="1"/>` For mixed columns, see [this guidance](http://dcs.library.virginia.edu/digital-stewardship-services/tei-encoding-guidelines/#cb).
- **`<div type="section">`** to wrap multiple items that belong together, for instance in the international or local news sections.
- **`<dateline>`** for datelines. There can only be one dateline per division. In the international news section, this means that you must make a new `<div type="item">` for each newswire report.
- **`<byline>`** for authors. There can only be one byline per division.
- **`<gap/>`** for holes in the text, **`<unclear>`** for illegible text (you can supply an attribute explaining why), and **`<supplied>`** for something that was illegible but which you figured out by finding the same thing in a different issue.
- pieces of articles that are continuous texts broken up by ads or between issues should be connected using xml:id and the next and prev elements, thus: if the articles are in the same issue, make their tags `<div type="item" xml:id="item1" next="item2">` and `<div type="item" xml:id="item2" prev="item1">`. If the articles are in different issues, make their tags `<div type="item" xml:id="item1" next="YYYY-MM-DD.xml#item2">` and `<div type="item" xml:id="item2" prev="YYYY-MM-DD.xml#item1">`.
- the **`<figure>`** element will be useful for the *Egyptian Gazette*, but I have not yet worked out how to use it.

## 4. Add advanced content tags
This is a more advanced undertaking. See the separate tutorial [here](/how-to/digitization/tagging-people-and-places-instructions/).