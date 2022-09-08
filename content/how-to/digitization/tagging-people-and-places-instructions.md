---
title: Tagging people and places
linktitle: Advanced tagging
toc: true
type: book
date: "2016-09-30"
draft: false
menu:
  digitization:
    parent: Digitization
    weight: 90

weight: 90
---
## Objectives

The greatest use for the encoded *Egyptian Gazette* will come in linking its content to other data sets. There are wonderful datasets listing people and places of the past.  This tutorial explains how we will link our project to those projects. To do so, we will use the Text Encoding Initiative (TEI)'s [rich schema for tagging people and places](http://www.tei-c.org/release/doc/tei-p5-doc/en/html/ND.html).

## 1. Tagging places
The basic tag that we will use is `<placeName>`. Full details of usage are [here](http://www.tei-c.org/release/doc/tei-p5-doc/en/html/ND.html#NDPLAC) and  [here](http://www.tei-c.org/release/doc/tei-p5-doc/en/html/ref-placeName.html).

The key element we will use to link our places to other date sets is `ref=`. We can use this to link to authorities such as wikidata, geonames, or [geohack](https://tools.wmflabs.org/geohack/geohack.php?pagename=Alexandria&params=31_12_N_29_55_E)

### Resources
- Goad fire insurance maps of [Alexandria](https://iiif.lib.harvard.edu/manifests/view/drs:15525296$3i) and [Cairo](https://iiif.lib.harvard.edu/manifests/view/drs:15525297$1i)
- [David Rumsey map collection](http://www.davidrumsey.com/luna/servlet/view/all?sort=Pub_List_No_InitialSort%2CPub_Date%2CPub_List_No%2CSeries_No)
- [Wikimapia](http://wikimapia.org)

## 2. Tagging persons
The basic tag we will use is `<persName>`. Full details of usage are [here](http://www.tei-c.org/release/doc/tei-p5-doc/en/html/ND.html#NDPER).

Work to link persons to references such as wikidata or viaf. For instance, you might describe Cromer thus:

```
<persName ref="https://www.wikidata.org/wiki/Q336487">
 <forename>Evelyn</forename>
 <surname>Baring</surname>, <roleName>1st Earl of Cromer</roleName>
</persName>
```

For persons not named, but who have a reference that you can supply (either an external authority or an xml:id), use `<rs>` (refering string).

## 3. Tagging events
To label an event, use a variant of the `<interp xml:id="">` tag.
