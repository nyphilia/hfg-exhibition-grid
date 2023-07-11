# HfG Exhibition Grid
Project showcase kiosk for semester exhibition

![screenshot](screenshot.png)

## Workflow
Throughout this document we will mention two user groups:
1. **Editor**: The person that organizes the kiosk, collects the content folders from the student and sets up the site.
2. **Student**: The student who built the projects

If you're the **Editor**, proceed to *Installation*. If you're a **Student**, proceed to *Creating a Content Folder*

## Installation
1. Download this project as .zip and unpack it
2. Choose the showcase folder with the correct type of your showcase (HTML, PDF or Video)
3. Start a webserver. We recommend using [Web Server for Chrome](https://chrome.google.com/webstore/detail/web-server-for-chrome/ofhbbkphhbklhfoeikjpcbhemlocgigb) as it allows for the easy creation of a webserver without having to hassle with Terminal commands. You may need to select the showcase folder as root folder within the app
4. After starting the webserver, open its IP in Safari or Chrome (usually `127.0.0.1:8887`)

## Preparing content folders
Rename all content folders from 1 to the amount of folders you have. The content will appear in the order of the folder names, i.e. folder 1 will be the first item in the grid, folder 2 the second etc.

## Populating a site with content
1. Within the `showcase` folder, find the `content` folder and enter it.
2. Delete the example content folder "1" and put the content folders the students supplied you with in here.
3. The `content` folder also contains a `content.js` file. Enter the names of the content folders here like this: `var contentFolders = ["1","2","3"];`

## Creating a Content Folder
1. Download this project as .zip and unpack it
2. In the main directory, find the content folder that matches your submission. The available types are:

- **showcase_html**, if you created a website
- **showcase_pdf**, if you created a PDF
- **showcase_video**, if you created a video

3. Download the folder and populate it as following:
- **title.txt** This file holds the title of your project. Enter it in raw text
- **description.txt** This file holds the description of your project. Enter it in raw text. If you don't have one, just leave it free
- **creator.txt** This file holds the creators of your project. Enter your name and the ones of your team mates here in raw text.
- **thumbnail.png** The thumbnail for your showcase. Create it with the template file in the `Thumbnail Generator` folder.
- **For HTML sites**: **index.html** The website that runs your project
- **For PDFs**: **pdf.pdf** The PDF file that shows your project. Leave the prefilled index.html in the folder
- **For Videos**: **video.mp4** The video that shows your project

Add any related folders you might need. **Make sure that the files names and extensions stay the same!** Then send your content folder to your **Editor**.

## Further customizations
Within the `content.js` you can set the amount of time of no user interaction until the kiosk should reset itself in miliseconds. The default value is 60000 (one minute).
