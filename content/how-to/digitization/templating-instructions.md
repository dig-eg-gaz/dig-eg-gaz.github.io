---
title: Templating instructions
linktitle: Templating
toc: true
type: book
date: "2019-09-19"
draft: false
menu:
  digitization:
    parent: Digitization
    weight: 30

weight: 30
---
## Objectives

While [features](/issues/features/) of the *Egyptian Gazette* were composed fresh each day, much of each issue consisted of templates reapplied with minor or no modifications from issue to issue. As we produce our marked-up version of the newspaper, we can save effort by reusing templates in our own work. We must remain alert to minor variations, however.

## 1. Identifying recurring features

The first step is to determine if you are looking at something that is a template. Advertisements, tables, and other material that is not free text is probably templated. Check these indexes to see if you can find something identical or similar to what you want to find:

- The complete catalog of advertisements is [here](/issues/advertisements/).
- The complete catalog of financial tables and other boilerplates is [here](/issues/templates/).

These indexes contain images of the templated items, links to TEI-XML documents representing the templated item, and (sometimes) a comment or two about the template. 

## 2. Using templates

Once you've identified the relevant template, you can paste its XML code into your own file. There are two ways to do this.

### 2a. Using content completion boilerplates

I've made a file that contains shortcuts to most of the boilerplates that you will need. (Note that it does not contain advertisements.) You can download it [here](https://raw.githubusercontent.com/dig-eg-gaz/boilerplates/master/dig-eg-gaz-code-templates.xml). Once downloaded, you can install the file in Oxygen XML Editor by opening the Preferences dialog box (Options > Preferences), then going to Editor > Content Completion > Code Templates. Now click the Import button, and select the file you have downloaded.

Once you have installed the content completion boilerplates, you can press Control + Space, and a drop down menu of templates will appear. Choose the template you need and it will automatically appear where your cursor was.

Next, customize the template content to match your issue's content. Often there will be no changes. Sometimes dates, names, or numbers will have to be changed. Sometimes the changes will be more complex. As you become more familiar with TEI-XML, you will get better at customizing the template.

Note that this content completion file will not be automatically updated. For the latest versions of boilerplates, consult the complete catalog, and follow the following procedure:

### 2b. Copy and paste from xml file

Once you've found the template you need, click the XML link. This will take you to a file in the dig-eg-gaz GitHub repository. Here you can copy the code you need to paste into your file. 

**Important**: Only copy the material contained within the `<body> </body>` tags--the rest of the file should not appear in your issue file. To do so, select the text like this:

![templateCopy](templateCopy.png)

Paste only this portion of the text into your issue document.

## 3. What if there's no template?

If you can't find a template that should be there, or if your version of an item is so different from the template that you think a new template is warranted, there are a few things you can do. 

- First, you can search the [repository of already-encoded issues](https://github.com/dig-eg-gaz/content) to see if someone has already produced a version of the material. 
- If you find it, or if you feel up to encoding it yourself, you can turn this into a new template so that everyone can save time. Upload the xml and an image of the feature to the [advertisements](https://github.com/dig-eg-gaz/advertisements) or [boilerplates](https://github.com/dig-eg-gaz/boilerplates) repository, and send a pull request. 
- Finally, if you can't find the material anywhere and it's too involved to reproduce it yourself, file an [issue](https://guides.github.com/features/issues/) at the [advertisements](https://github.com/dig-eg-gaz/advertisements/issues) or [boilerplates](https://github.com/dig-eg-gaz/boilerplates/issues) repositories, insert a `<!-- missing template -->` comment with a few details into your document, and move on.

## 4. An overview of "features" from page to page and day to day

For a general summary of recurring features, see the tables [here](/issues/features/). Every numbered page of the _Gazette_ held similar material every day. The slides below offer an overview of the format over a typical week in July 1905. Page numbers are indicated on the bottom right. The main boilerplate is six pages long. On Wednesday and Saturday, when issues are eight pages, the extra pages are the fourth and fifth pages. Pages 6-8 of extended editions correspond to pages 4-6 of regular editions.

{{< gdocs src="https://docs.google.com/presentation/d/e/2PACX-1vSoNMUJRV31l_qJ-hWRQwU3JHdGi8wLNv5nEndc6eeQWcRqbo9womcWCRDlgRJmumWR7i-RL5G2rFRv/embed?start=true&loop=false&delayms=3000" >}}

