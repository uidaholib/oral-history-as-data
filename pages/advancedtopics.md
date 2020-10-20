---
layout: page
title: Advanced Topics  
object-id: notes
permalink: /advancedtopics.html
---
# {{page.title}}

- [Using the tool offline](#using-the-tool-offline)
- [Customizing the Site](#customizing-the-site)
- [Serve the site from another location](#serve-the-site-from-another-location-not-github-pages)
  - [Serving on another web server](#building-the-flat-files-and-copying-to-a-server)
  - [Serving a customized domain from GitHub](#using-dns-records-to-serve-the-github-repository-at-another-url)


## Using the tool offline

If you'd like to do this on your computer, using Jekyll's built in development server, you'll need to install Jekyll (which requires Ruby). Instructions for installations can be found on the [CollectionBuilder Software page](https://collectionbuilder.github.io/docs/software.html) or on the [Lib-STATIC How-to pages](https://lib-static.github.io/howto/).

{:.btn .btn-outline-primary .text-white .mb-3}
[More on Jekyll can be found here.](https://jekyllrb.com/)

## Customizing the Site

The site is built using [Bootstrap](https://getbootstrap.com). The layouts and styles of the buttons, etc. are set up using the classes and javascript interactions allowed. 

To edit the what links appear in the header, edit the `nav-configuration.csv` in the `\_data\` folder.

All the code is available to be edited. To get started editing the header and navigation, look at the `site-banner.html` and `site-nav.html` in the `\_includes\` folder. 

To edit any of the layouts for the various pages, check out the files in the `\_layouts\` folder. 

Here's a Bootstrap 4 Tutorial if you want to learn more](https://www.w3schools.com/bootstrap4/)
[Here's a Bootstrap 4 Tutorial if you want to learn more](https://www.w3schools.com/bootstrap4/)

## Serve the site from another location (not GitHub Pages)

### Building the flat files and copying to a server

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

### Using DNS Records to serve the GitHub repository at another url.

- GitHub has a lot of information about [how to configure a custom domain for your website](https://docs.github.com/en/free-pro-team@latest/github/working-with-github-pages/configuring-a-custom-domain-for-your-github-pages-site).