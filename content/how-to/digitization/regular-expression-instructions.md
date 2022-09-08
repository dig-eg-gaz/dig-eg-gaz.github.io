---
title: Regular expressions instructions
linktitle: Regular expressions
toc: true
type: book
date: "2016-09-30"
draft: false
menu:
  digitization:
    parent: Digitization
    weight: 110

weight: 110
---
Regular expressions (regex) is a very useful means of working with serial data which repeats similar information using similar formats.

[Regexr](https://regexr.com/) is a great place to learn about and try out regular expressions.

## Using regex in Oxygen

You can use regex in the Find/Repace in Files tool when you enable the Regular Expression option in it. 
Some examples of commonly used regex codes:

- Search `\d+ \w+ \w+ ` for patterns like "100 tons cotton"
- Search `\W\w+ \W\w+ ` for personal names
- Search `at [A-Z]\w+ ` for locations (Remember to enable Case Sensitive)

## Using regex in Atom

To put `<persName>` around passenger names in a list: find `Mr. [A-Z][a-z, 0-9]+,` replace with `<persName>$&</persName>`.

<!-- To convert `<p>Budapest, January 4.</p>` to `<dateline>Budapest, January 4.</dateline>`: find `<p>[A-Z][a-z]+, [A-Z][a-z]+ [0-9]+\.<\/p>` and replace with `<dateline>$&</dateline>`. -->

## Cleaning XPath results

1. Select all, copy, and paste results into your plain text editor.

2. First, let's remove the lines that start with "XPath location," "Start location," and "End location," because we won't need these results. Open find and replace. Click the Regex option, then use this regex to find the first of these results: `XPath location: .+\n`. *Note*: if you're using Windows, you may have to replace the `\n` (new line indicator) at the end of this string with `\r\n`, which is how Windows sometimes indicates new lines.

Once you've selected all of these "XPath location" lines, replace them with nothing (i.e., leave the replace box empty). Click Replace All.

Now you can do the same for `Start location: .+\n` and `End location: .+\n`

3. Remove the file location that precedes the issue date. Find `System ID: /Users/whanley/GitHub/DEG-content/` (this will be different on your computer--just select everything that comes before the date filename). (You may need to turn off Regex in order to find this string text.) Leave the replace box empty, then click Replace All.

4. Now we replace what comes between the date and the results. Turn Regex back on, then find `.xml\nDescription: ` (or `.xml\r\nDescription: ` if you are using Windows) and replace with `\t`. Replace All.

5. If you have empty lines in your file, you can remove them by finding `\n\n` (or `\r\n\r\n`) and replacing it with `\n`.

6. You might have a bit of garbage left over at the beginning and end of the file. Delete this. Now you will have a tab-separated, two-column table that you can paste into a spreadsheet.

## Using regex in Microsoft word

Say you are trying to make a table of the results that you exported from Oxygen.

Import these results into a Word document. Then use Edit > Find > Advanced Find and Replace.

1. Find two paragraph marks (^p^p), and replace with @@.
2. Find one paragraph mark (^p), and replace with comma.
3. Find @@, and replace with paragraph mark (^p).
4. Select all text, then use Table > Convert > text to table.
