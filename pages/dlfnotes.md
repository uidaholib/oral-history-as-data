---
layout: howto
title: Notes, Common Issues, and Next Steps  
object-id: notes
permalink: /dlfnotes.html
---
Thank you very much for watching the presentation. Here is some additional information to help you on your way!

- [Notes](#notes)
- [Common Issues](#common-issues)
    - [The Website Isn't Showing Up!](#the-website-isnt-showing-up)
    - [My Audio/Video File isn't Connected](#my-audiovideo-file-isn't-connected)
    - [My transcript pages aren't showing up](#my-transcript-pages-arent-showing-up)
    - [The Visualization isn't working](#the-visualization-isnt-working)
    - [Other Problems](#other-problems)
- [Next Steps](#next-steps)
    - [Using the tool offline](#using-the-tool-offline)
    - [Customizing the Site](#customizing-the-site)
    - [Serve the site from another location](#serve-the-site-from-another-location-not-github-pages)


## Notes

- Much of the documentation followed for the presentation was prepared by Michael Decker while serving as a Graduate Assistant in the CDIL. 
- My colleagues Olivia Wikle and Evan Williamson have contributed code, support, and inspiration for the Oral History as Data Project. 

## Common Issues

### The Website Isn't Showing Up!

This problem is usually caused by having the wrong settings in the "URL settings" section of the _config.yml. 

Check the variables provided and make sure that the url and baseurl are correctly formatted. 

{:.btn .btn-outline-primary .text-white .mb-3}
[More in the documentation](https://uidaholib.github.io/oral-history-as-data/howto/deploy.html#step-2-edit-your-url-settings-url-baseurl-and-repository)

### My Audio/Video File isn't Connected

- Check the markdown file for your transcript. 
    - Is the correct AV Source designated? 
    - if it is, is the source in lowercase? It needs to be!
- Check the AV ID and see if that matches the ID you are trying to connected. Soundcloud has a specific way of connecting, and we need either a full link or relative link (if the mp3 is stored on the website).
- Check the permissions on your file. 
    - For instance, YouTube videos need to be either unlisted or public for the tool to access them. 

{:.btn .btn-outline-primary .text-white .mb-3}
[More on connecting AV files here.](https://uidaholib.github.io/oral-history-as-data/howto/configurethesite.html#optional-connect-the-transcript-to-an-audio-or-video-file-using-av_source)

### My transcript pages aren't showing up

- Is your CSV file correctly formatted?
    - check this by going to the file on the GitHub.com website and seeing if it shows up on the page in a table. 
    - if it doesn't, and you get an error message from GitHub about the CSV, check the line it references and try to fix it. 
- Is the content in the right format and listed in the right columns?
    - The content needs to be in the `words` field.

{:.btn .btn-outline-primary .text-white .mb-3}
[More on setting up your transcript CSVs correctly here.](https://uidaholib.github.io/oral-history-as-data/howto/prepareyourdata.html)

### The Visualization and/or browsing dropdown isn't working

- make sure you have a `filters.csv` file in your `_data\` folder. 
- make sure that file is correctly formatted.
- make sure that the shorthand codes you use in your transcript CSV match up with the information in that file. 

More on setting up your filters.csv correctly here. 

### Other Problems

- If you're running into serious issues, please let me know! You can either [make an issue on the GitHub Repository](https://github.com/uidaholib/oral-history-as-data/issues), or just email me at dbecker@uidaho.edu. 

## Next Steps

### Using the tool offline

If you'd like to do this on your computer, using Jekyll's built in development server, you'll need to install Jekyll (which requires Ruby). Instructions for installations can be found on the [CollectionBuilder Software page](https://collectionbuilder.github.io/docs/software.html) or on the [Lib-STATIC How-to pages](https://lib-static.github.io/howto/).

{:.btn .btn-outline-primary .text-white .mb-3}
[More on Jekyll can be found here.](https://jekyllrb.com/)

### Customizing the Site

The site is built using [Bootstrap](https://getbootstrap.com). The layouts and styles of the buttons, etc. are set up using the classes and javascript interactions allowed. 

To edit the what links appear in the header, edit the `nav-configuration.csv` in the `\_data\` folder.

All the code is available to be edited. To get started editing the header and navigation, look at the `site-banner.html` and `site-nav.html` in the `\_includes\` folder. 

To edit any of the layouts for the various pages, check out the files in the `\_layouts\` folder. 

Here's a Bootstrap 4 Tutorial if you want to learn more](https://www.w3schools.com/bootstrap4/)
[Here's a Bootstrap 4 Tutorial if you want to learn more](https://www.w3schools.com/bootstrap4/)

### Serve the site from another location (not GitHub Pages)

##### Building the flat files and copying to a server

In order to build the directory that serves up the entire website, you need to use the tool on the desktop, typically using a terminal and a text editor. 

Jekyll has two main commandline commands to serve and build a jekyll site. 

- `jekyll s` - builds a development test server on your computer and provides a local website for you to look at the changes you make as they will appear in browser. This will use your `baseurl` setting in the `_config.yml` file to create relative links

*To Build the site you'll need to use:*

- `jekyll build` - builds the site to work on any url + directory you might like to put it on. These are determined by the `url` and `baseurl` variables in the `_config.yml` file.
    - These files will be built in a `_site` directory. 
        - first, enter `jekyll build` in the commandline
        - after the process finishes it will note that in the command line
        - go to the `_site` directory at the root of your project repository and copy all the files and folders within the directory.
        - paste those files and folders into the directory where you'd like to serve the files. 
    - You need to anticipate where the site will be served. So, if it's going to be served at `example.com` you would need to  have the `url` variable filled into be `https://www.example.com` and the `baseurl` should be blank.
    - Example, if we're serving a website at www.lib.uidaho.edu/oralhistory/, I would change the `url` to be `https://www.lib.uidaho.edu/` and the baseurl to be `oralhistory/`

###### Using DNS Records to serve the GitHub repository at another url.

- GitHub has a lot of information about [how to configure a custom domain for your website](https://docs.github.com/en/free-pro-team@latest/github/working-with-github-pages/configuring-a-custom-domain-for-your-github-pages-site).