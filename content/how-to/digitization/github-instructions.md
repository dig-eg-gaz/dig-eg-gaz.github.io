---
title: GitHub instructions
linktitle: GitHub
toc: true
type: book
date: "2016-09-30"
draft: false
menu:
  digitization:
    parent: Digitization
    weight: 40

weight: 40
---

## Objective
We will manage our digitization of the Egyptian Gazette using GitHub. This tutorial gives you instructions about how to submit your own work to our shared repositories.

## 1. What is GitHub?
GitHub is a tool to manage versioning and collaboration in coding projects large and small. It's built on [git](https://en.wikipedia.org/wiki/Git) software, and offers a bunch of useful social and communication tools in its user interface. Each of us will create an individual account where we'll store and refine our work until it's ready to upload to the [dig-eg-gaz organization repositories](https://github.com/dig-eg-gaz).

## 2. How to access GitHub
You can approach GitHub three ways:

- using a web browser to access [github.com](https://github.com/),
- using the [GitHub Desktop](https://desktop.github.com/) client , or
- using [the command line](http://programminghistorian.org/lessons/intro-to-bash).

We'll be using the Desktop client mostly, but in a pinch you can use the web browser.

## 3. How to use the organization repository and your own fork of it
1. Navigate to the organization [content repository](https://github.com/dig-eg-gaz/content), and **fork** the repository by clicking on the "fork" icon on the top right. You will be offered the chance to fork the repository under your own username--do so. This will make a copy of the repository in your own GitHub account.
2. Clone this repository in your Desktop.
3. In GitHub Desktop, right click the "content" repository, and choose "Show in Finder." This will show where the content files you've just cloned are stored on your hard drive. Move your xml files here, and continue to edit and save them in this location. Desktop will help you to send these edits to Github.
![show in finder](content-show-in-finder.png)
4. When you're ready to sync your changes with the GitHub cloud, write a summary of your changes (e.g., "creating page 1"), hit "Commit to Master", then hit "Fetch origin" (on the top right). This will backup your work onto your fork on GitHub's servers.
![fetch origin desktop](fetch-origin-desktop.png)

## 4. How to submit your deliverables
When your page files are complete, you can fold them from your own fork into the **master** organization content repository by sending me a **pull request**. You do this by navigating (on the github website) to *your fork* of the content repository. If it says "This branch is 1 commit ahead," you can submit a pull request by clicking the "new pull request" button on the top left above your list of files. Follow the instructions and keep clicking until the pull request is submitted.
![new pull request](new-pull-request.png)
I will then see the pull request and either merge your files into the organization's content or request that you change something before doing so. If you want to check the status of your pull requests, scroll all the way to the top of the github web page. Click on "Pull requests" in white letters on a black background. You will then see a list of the pull requests you've submitted.

## 5. How do I make sure that my content fork is up to date?
In the screenshot above, you'll notice the caption "This branch is 1 commit ahead, 98 commits behind dig-eg-gaz:master." "Commits ahead" is work that you've done and will (or have already) submitted in a pull request. Once it's merged into the master content repository, your fork will be "no commits ahead". 

"Commits behind" represents work that your colleagues have done and that has been merged into the master content repository _after_ you first made your fork. These updates don't make their way into your fork automatically. Normally this is not big deal, as you aren't working on those files anyway. But when it comes time to do your querying and analysis of the whole repository, it's very important to make sure that you are working on an up-to-date version of the master content files. 

When you look at your fork of the `dig-eg-gaz/content` repository on the github website, you will see a line comparing your repository to the organization repository:
![not up to date](250-commits-behind.png)
If you are ahead, click the "new pull request" button above the status report and ask the organization to merge your changes.

If you are behind:

1. click "pull request" on the same line and to the right of the status of the report.
2. You need to manipulate things so that your fork is the "base repository" and the `dig-eg-gaz/content` is the "head repository". I'm not completely sure how to accomplish this...
3. You will then be taken to a screen that allows you to create a pull request. Do so.
4. This pull request will now appear on the "pull requests" tab of your fork of the content folder.
![pull requests](pull-requests-tab.png)
Click on the tab, and on the pull request, and then merge the pull request.
5. Your fork should now be up to date--the status line will confirm this.

## 6. Resources
These Github tutorials might be useful:

- [Github flow](https://guides.github.com/introduction/flow/): describes branch, commit, pull, etc. 5 minute read.
- [Hello world](https://guides.github.com/activities/hello-world/): step-by-step explanation of key functions via web interface. 10 minute read.
- [Understanding Github](http://readwrite.com/2013/09/30/understanding-github-a-journey-for-beginners-part-1/): very clear introductory discussion, focusing on command line interface.
