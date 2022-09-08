---
title: Microfilm instructions
linktitle: Microfilm
toc: true
type: book
date: "2016-09-30"
draft: false
menu:
  digitization:
    parent: Digitization
    weight: 10

weight: 10
---

## Objective
This tutorial explains how to produce high-quality, [OCR](/how-to/digitization/OCR-instructions/)-readable images from microfilm of a historical newspaper. **Note:** Library staff may offer you some help in using the microfilm readers, but they are not responsible to do the work for you. This tutorial explains everything you need to know to do this task.

## 1. Setup
1. Get film NP 486 for the appropriate month and year from the reserve desk in the basement in Strozier. You can sign it out for two hours. Each film contains three months' worth of issues. You might have to scroll through a lot of film to find your date.
2. Log on to one of the six microfilm-enabled computers, and open the "Microform PowerScan/PowerScan" program. Indicate that you are using microfilm or, if you are using PowerScan 2200, select the "Expert User + New Features" mode so you can change the resolution. Thread the film into the microfilm reader (a "ScanPro 1000/2200"), carefully following the threading route mapped on the table or the machine itself. Run a bit of film through the machine until you begin to see page images--the first foot of film is only black.
3. Familiarize yourself with the controls at the bottom of the program. The "Motorized Roll Film Control" allows you to move through the film and find the issue you need. The toggle switch at the top moves the film slowly, and is useful to make exact adjustments. The larger "Adjust Image" menu has numerous controls. If your image is only displaying as half screen, click the "Film Orientation" button (or "Fill to Width" under the "Home" menu if you are using Powerscan 2200) and it will shift to full screen. You can play with the zoom until you see a whole page on the screen--you may have to move the carriage in the microfilm reader itself to center the image. You can focus, change the brightness, and so on, which will give you a more readable result.

## 2. Scan the page in quarters
1. In order to produce a high-quality, OCR-ready image, it is necessary to scan the page in quarters, then stitch the image together. Zoom in on the image until the screen shows just the top left-hand quarter of the page, thus:
![quarter page example](quarter-page-example.jpg)
Make sure that you leave a bit of overlap, so that the image stitching software can do its task.
2. Change the shape of the green box, which shows the part of the image that you will save to a file, so that it contains the edges of the print. Make sure that the image is straight, balanced, and focused.
3. Now you are ready to save it as an image file. Under the Scan/Print tab, change the scan resolution to 600dpi. Press "Scan to Drive #1." Name your file following the standard dating format plus page number plus a suffix for the top left hand corner (YYYY-MM-DD-p1a). Choose file type jpg. Then proceed to scan the bottom left hand corner (p1b), the top right (p1c), and the bottom right (p1d).

## 3. Stitch the quarters
1. Stitch the four quarters into a single high-resolution file using the [Microsoft Image Composite Editor](http://research.microsoft.com/en-us/um/redmond/projects/ice/). The program is loaded on all of the scanning computers at Strozier. If you use a Windows computer, it is free to download for your own computer. When you open the program, click "New Panorama," import the four quarter images you just produced, click "Stitch," then click "Export." Choose image quality "superb," and save the file with the name "YYYY-MM-DD-p1.jpg". This is the file that you will use for subsequent work--save it to your hard drive.
2. Go ahead and do the same for all the pages of the issue. **Note:** You may find that certain pages (often page 1) are doubled on the microfilm. When this is the case, you only need scan one version of the doubled page.

## 4. Save your files
1. Find the stitched image files you've created on the computer's hard drive, and copy them to a USB key, save them to Dropbox, or save them some other way. Do not simply leave them on the microfilm computer. You do not need to save the quarter page images.
2. Return the microfilm to the checkout desk--your classmates will need to find it.

## 5. Upload your images
1. Each image file should be between 2MB and 10MB in size. If your files are larger than that, you will have to compress them.
2. Once you are satisfied with your images, upload them directly to the appropriate subfolder within the [page-images repository](https://github.com/dig-eg-gaz/page-images) repository on GitHub. There are many subfolders (one for each quarter of each year). Make doubly sure before *before you upload* that your images are named exactly according to this format: `YYYY-MM-DD-p1.jpg`. 

### Troubleshooting
Sometimes the microfilm hardware fails to function. When this is the case, follow these instructions (courtesy Malcolm Shackelford of FSU libraries): Those MF machines are prone to fits, but the cure is nearly always to

1. stop the microform viewing/scanning application.
2. turn off the MF machine using the switch on the rear left
3. detach and reattach the firewire cable from both the MF machine and the computer
4. fire up the machine, then the scanning program

Doing the above makes sure we don't have a loose cable, and reminds Windows that the device is there and alive.