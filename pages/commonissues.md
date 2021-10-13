---
layout: howto
title: Common Issues
object-id: notes
permalink: /commonissues.html
---
# {{page.title}}

- [The Website Isn't Showing Up!](#the-website-isnt-showing-up)
- [My Audio/Video File isn't Connected](#my-audiovideo-file-isn't-connected)
- [My transcript pages aren't showing up](#my-transcript-pages-arent-showing-up)
- [The Visualization isn't working](#the-visualization-isnt-working)
- [Other Problems](#other-problems)

## The Website Isn't Showing Up!

This problem is usually caused by having the wrong settings in the "URL settings" section of the _config.yml. 

Check the variables provided and make sure that the url and baseurl are correctly formatted. 

{:.btn .btn-outline-primary .text-white .pb-3}
[More in the documentation](https://uidaholib.github.io/oral-history-as-data/howto/deploy.html#step-2-edit-your-url-settings-url-baseurl-and-repository)

## My Audio/Video File isn't Connected

- Check the markdown file for your transcript. 
    - Is the correct AV Source designated? 
    - if it is, is the source in lowercase? It needs to be!
- Check the AV ID and see if that matches the ID you are trying to connected. Soundcloud has a specific way of connecting, and we need either a full link or relative link (if the mp3 is stored on the website).
- Check the permissions on your file. 
    - For instance, YouTube videos need to be either unlisted or public for the tool to access them. 

{:.btn .btn-outline-primary .text-white .mb-3}
[More on connecting AV files here.](https://uidaholib.github.io/oral-history-as-data/howto/configurethesite.html#optional-connect-the-transcript-to-an-audio-or-video-file-using-av_source)

## My transcript pages aren't showing up

- Is your CSV file correctly formatted?
    - check this by going to the file on the GitHub.com website and seeing if it shows up on the page in a table. 
    - if it doesn't, and you get an error message from GitHub about the CSV, check the line it references and try to fix it. 
- Is the content in the right format and listed in the right columns?
    - The content needs to be in the `words` field.

{:.btn .btn-outline-primary .text-white .mb-3}
[More on setting up your transcript CSVs correctly here.](https://uidaholib.github.io/oral-history-as-data/howto/prepareyourdata.html)

## The Visualization and/or browsing dropdown isn't working

- make sure you have a `filters.csv` file in your `_data\` folder. 
- make sure that file is correctly formatted.
- make sure that the shorthand codes you use in your transcript CSV match up with the information in that file. 

More on setting up your filters.csv correctly here. 

## Other Problems

- If you're running into serious issues, please let me know! You can either [make an issue on the GitHub Repository](https://github.com/uidaholib/oral-history-as-data/issues), or just email me at dbecker@uidaho.edu. 
