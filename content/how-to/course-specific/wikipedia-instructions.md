---
title: Wikipedia instructions
linktitle: Wikipedia
toc: true
type: book
date: "2020-04-23"
draft: false
menu:
  course-specific:
    parent: Course specific
    weight: 5

weight: 5
---

Much of the information that Wikipedia offers us about turn-of-the-century Egypt is derived from earlier, top-down sources (for example, the [_Encyclopedia Britannica_ of 1911](https://en.wikipedia.org/wiki/Encyclop%C3%A6dia_Britannica_Eleventh_Edition)). The _Egyptian Gazette_ contains a wealth of microhistorical data that can enrich the 

## 1. Identify a subject

The first step is to find a Wikipedia page that needs your help. One way to get there is to use category pages, such as:

- [Egyptian politician stubs](https://en.wikipedia.org/wiki/Category:Egyptian_politician_stubs) (a stub is "an article deemed too short to provide encyclopedic coverage of a subject")
- [People from Cairo](https://en.wikipedia.org/wiki/Category:People_from_Cairo)
- [Pashas](https://en.wikipedia.org/wiki/Category:Pashas)

If you are working on a person stub, you can search for that individuals in the _Digital Egyptian Gazette_ content repository. Identify a news story that informs us of an important event in their lives, ideally something unaccounted for on the page. (Of course, you can also add the _Gazette_ as a reference in support of information already given in Wikipedia.)

You might wish to work on an event or a place, or to create a new Wikipedia page for someone of significance. All of this is worthwhile work.

## 2. Edit the page

Sign up for Wikipedia and log in. Click "edit" near the top right of the page, and you will see the page's text encoded in [wikitext](https://en.wikipedia.org/wiki/Help:Wikitext) (Wikipedia's syntax). It's a simple language, not so different from Markdown, and there are lots of tips and tutorials available--here's a [good place to start](https://en.wikipedia.org/wiki/Help:Editing). Proceed to add the necessary text to the page.

## 3. Cite your source

At the end of the information that you add, provide a reference to your source article in the _Egyptian Gazette_. Use this basic format (updated to reflect your source):

```
<ref>{{cite news |author=<!--Staff writer(s); no by-line.--> |title=Personal and Social. |url=https://raw.githubusercontent.com/dig-eg-gaz/page-images/master/1906-page-images-4/1906-12-27-p3.jpg |work=The Egyptian Gazette |date=27 December 1906}}</ref>
```

(The url I've linked to is the page image of the article I've used.)

## 4. Save your edit

You will want to preview it first to check if the format is correct. You might also wish to watch the page, just in case someone removes your change--when this happens, it often happens in the first 24 hours.

## 5. Let me know what you've edited

The best way to do this is to send me the link to your "user contributions" page. My link looks like this: `https://en.wikipedia.org/wiki/Special:Contributions/Will_Hanley`.

# An example

I found this mention of the funeral of the daughter of Joseph Cattaui in the "Personal and Social" section on page 3 of the December 27, 1906 issue.

![funeral blurb](/img/cattaui-funeral.png)

This prominent businessman has [his own Wikipedia page](https://en.wikipedia.org/wiki/Joseph_Cattaui). It names some of his family members in the box on the right, but I'm not sure which daughter it is who died. I decided to add a new section mentioning this information about his private life. Here's the code I used:

```
==Personal life==

Cattaui's daughter died of typhoid fever at the age of 18 at the end of December, 1906.<ref>{{cite news |author=<!--Staff writer(s); no by-line.--> |title=Personal and Social. |url=https://raw.githubusercontent.com/dig-eg-gaz/page-images/master/1906-page-images-4/1906-12-27-p3.jpg |work=The Egyptian Gazette |date=27 December 1906}}</ref>
```

The edit is recorded in the page history [here](https://en.wikipedia.org/w/index.php?title=Joseph_Cattaui&type=revision&diff=952696886&oldid=950009046).