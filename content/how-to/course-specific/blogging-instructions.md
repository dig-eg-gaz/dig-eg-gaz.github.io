---
title: Blogging instructions
linktitle: Blogging
toc: true
type: book
date: "2019-10-08"
draft: false
menu:
  course-specific:
    parent: Course specific
    weight: 1

weight: 1
---

## 1. Fork the repository

Fork a copy of the organization [blog-posts](https://github.com/dig-eg-gaz/blog-posts) repository on your personal github account. Do this by clicking on the "fork" icon on the top right. You will be offered the chance to fork the repository under your own username--do so. This will make a copy of the repository in your own GitHub account, in which you should save your draft blog posts.

## 2. Set up your post

Make a duplicate of the `YYYY-MM-DD-name` folder, **leaving the original in place**. Rename the _duplicate_ folder with today's date and your name. This is the folder where you will put your blog post. The folder contains a file named `index.md`. Open this file in a plain text editor such as Atom or Sublime Text.

## 3. Fill in the header

The header (the material in the opening lines of the document, between the two --- lines) is very important. It tells the website how to treat your blog post. Replace the comments (`<!--insert-->`) in the header. Give your post a title and provide a one to two sentence summary. For author, give your full name with no spaces (for me, this is `[willhanley]`). List a few tags that reflect the subject matter that your post covers. Enter the date. Keep the category `[curiosities]`. 

## 4. Choose a feature image

Choose an image that you would like to appear to promote the post on the main page of the website. Name that image `featured.jpg` or `featured.png` (depending on the file format), and add it to your blog post folder (replacing the `featured.png` file that's already there). You do not need to add any more information about the image to the header, other than giving it a caption in the appropriate section. (For more on images, see number 5 below.) 

## 4. Write a post in markdown and add images

You will write your text using [Markdown](https://en.wikipedia.org/wiki/Markdown), a very simple markup language but a different one from xml, which you are using for the newspaper pages. Here's a [tutorial](http://www.markdowntutorial.com/) and here's a [cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet). Aim for at least 200 words, but it's fine if you write more. Integrate some links into your post (especially to previous blog posts on similar topics), and use an image or two.

## 5. Working with images

Include an image clipped from your issue of the paper, and any other images that might add to the impact of your post. If you are using an image that you find on the internet, make sure that you have the right to reuse it, and download the image (don't just link to it). 

Your feature image will not appear in the body of your post unless you insert it, using this syntax: 

`![label](featured.jpg)`

To include other images in your post, add the image file to the folder. Then, add a line to the blog post in the following format: `![Image label](image-file-name.png "Caption")`. The "Caption" information is optional, but encouraged.

## 6. Complete your author page

I want to give you credit on the website for the work you do. In order to tell everyone who you are, change the `YourNameNoSpaces` folder in your blog folder. Rename it using your first and last name without spaces. Then open the index file within the folder and add your own information, as you like. Remember to supply your github username. You can also replace the avatar image with one of your own choosing if you like (just make sure it's square).

## 7. Send a pull request to the group repository

When your blog post and image are ready, you can fold them back into the organization content repository by sending me a **pull request**. You do this by clicking the "new pull request" button the top left above your list of files. I will then see the pull request and either merge your files into the organization's content or request that you change something before doing so.
