---
layout: howto
title: How To Write a How-To
---

All of our how to files will be written in markdown. Here's a quick reference: 

- [Markdown Reference](https://commonmark.org/help/)

## Intro and Initial Header

Each how-to can start with a general introduction if needed, after which, you should start the steps with a header 2, or <h2> so start the line with "##" and write the title of the section. 

## This is a header 2

There may be a couple sections with header 2s needed, or you might not need any. 

## Steps

Each step should be a header 3, or <h3>, so you should start those lines with "###" and write "Step X - [title of step]

### This is a header 3

Within the steps, you should be separating out actions by making them list items. In markdown, you do this by starting the line with a dash ('-') and then writing the instructions. 

- this is an action list itme

Keep each action short and add an image if it makes sense. 

## Adding Images

### How to name and where to Put the Images

Name all images using only lowercase characters. Include no spaces in the filename, or anything else weird. 

Add the image to a folder inside the '/images/howto/' folder that pertains to your section. 
So if you're talking about 'git' put your images in a folder called 'git' -- if you need to create that folder, that's fine. 
Folder names should also be lowercase, no spaces, or anything else weird.

You will then reference that folder in the include explained below. 

### How to include the images in your Markdown

We will be adding images by using a [jekyll include](https://jekyllrb.com/docs/includes/). The include looks  like this example: 

{:.pl-4}
`{%raw%}{% include bootstrap/figure.md img="rubyinstaller-download.png" caption="Download Ruby+Devkit 2.6.5-1 (x64)" alt="a screenshot of the first section of the Ruby Installer website" %}{%endraw%}`

This include pushes your variables -- which in this example are "img", "caption", and "alt" -- into a [Bootstrap figure](https://getbootstrap.com/docs/4.0/content/figures/). 

The "img" variable should reference your images location, starting with '/howto/'. 

The "caption" variable will be written below the image included. You should use the caption to briefly describe the image and add an instruction or other reference to the step.

The "alt" variable should be a verbose description of the image for screen readers. 

### Adding a Boostrap Alert

Boostrap alerts are added by including a class for the paragraph you are writing. To do this you put brackets above the paragraph like this: {:.alert alert warning}. I'll give examples below. 

{:.alert .alert-warning}
This is an alert warning

Written like this: 

`{:.alert .alert-warning}`

`This is an alert warning`

{:.alert .alert-info}
This is an alert info

{:.alert .alert-success}
This is an alert success

{:.alert .alert-danger}
This is an alert danger

{:.alert .alert-primary}
This is an alert primary

You can use this method to add any Bootstrap classes you might want to use. 

{:.card .col-md-3 }
I made this a small card by adding {:.card .col-md-3}


