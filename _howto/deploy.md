---
layout: howto
title: How To Edit Your _config.yml File
---

When you design your website you'll need to utilize the *_config.yml* folder to help establish the working parameters of your page, the basic information that inhabits it, and the general layout your visitors interact with. 

{:.alert .alert-warning .mb-4}
NOTE: when you are navigating through the _config.yml file, you will notice lines that being with hashtags. These are "[comments](https://www.cs.utah.edu/~germain/PPS/Topics/commenting.html)" that provide useful information about how various lines effect your page. 

## Step 1: Open the `_config.yml` file

- First, find the *_config.yml* file in your base directory, which is the directory that opens when you first open the repository in github.  
{% include bootstrap/figure.md img="howto/configscreen.png" caption="image of _config.yml file found on main page of repository" alt="image of config folder" class="w-50" %}

- Once you open up the folder, you'll need to edit the file. Click on the pencil icon at the top right corner of the page to edit the file. 
{% include bootstrap/figure.md img="howto/edit_pencil.png" caption="" alt="image of config folder" class="w-50" %}

## Step 2: Edit your URL Settings (*url, baseurl*, and *repository*)

{:.alert .alert-info}
The URL settings control how the site generator (Jekyll!) builds the urls on your web pages. These are extremely important, whether you're going to serve this up using GitHub Pages or publish the site on another server. We demonstrate below how to set up the site to be served via [GitHub Pages](https://pages.github.com/).

{% include youtube/embed.html  video-id="OAl_pcWjBwk" title="Editing URL Settings" display="d-none d-md-block" %}

- First, you'll need to change your url. To do this, delete "uidaholib" from the `url` line, and replace it with your GitHub username. 
{% include bootstrap/figure.md img="howto/beforename.png" caption="url before edit" alt="url line in config folder before being edited" class="w-50" %}

{% include bootstrap/figure.md img="howto/aftername.png" caption="url after edit" alt="url line after editing" class="w-50" %}

- Now you'll need to edit your `baseurl`. After the forward slash you'll delete "oral-history-as-data" and type the name of your repository. 
{% include bootstrap/figure.md img="howto/basebefore.png" caption="baseurl line before edit" alt="image of baseurl line before edit" class="w-50" %}
{% include bootstrap/figure.md img="howto/baseafter.png" caption="baseurl line after edit" alt="image of baseurl line after edit" class="w-50" %}

- Finally, we'll edit your `repository` line, which will provide a link back to your code from the footer of your site. Erase the text that reads "uidaholib" and replace it with your username. Then erase the string that reads "oral-history-as-data" and replace it with your repository name. 

{% include bootstrap/figure.md img="howto/beforerepos.png" caption="repository before edit" alt="repository line before editing" class="w-50" %}
{% include bootstrap/figure.md img="howto/afterrepos.png" caption="repository after edit" alt="repository line after editing" class="w-50" %}

## Step 3: Editing Site settings

{:.alert .alert-info}
The site settings control what appears in the website's banner, both the bit title of the site and the tagline underneath it.  The description is put in the code of each page to enable people to find your site on Google or other search engines. 

{% include youtube/embed.html  video-id="gTJpfunqapQ" title="Editing Site Settings" display="d-none d-md-block" %}

##### Editing *title, tagline,* *and description* 

- Now scroll down to the next section in this folder titled *site settings*. Go to the first line called *title* and change "Oral History (as) Data" to what ever you would like to call your site. 
{% include bootstrap/figure.md img="howto/beforetitle.png" caption="title before edit" alt="title line before editing" class="w-50" %} 

{% include bootstrap/figure.md img="howto/aftertitle.png" caption="title after edit" alt="title line after editing" class="w-50" %}

- Now we're going to edit the *tag line*, which is a short banner that will run across your site next to the title. You're going to replace the text next to *tagline* that says "analyze and publish coded oral history and qualitative interviews" with whatever site description you would like. 
{% include bootstrap/figure.md img="howto/beforetag.png" caption="tagline before edit" alt="tagline before editing" class="w-50" %}

{% include bootstrap/figure.md img="howto/aftertag.png" caption=" tagline after edit" alt="title line after editing" class="w-50" %}

- In the same way as above, go ahead and edit the `description` variable. This should be a longer description of your site, with keywords, dates and other material included. This will be what site indexers like Google ingest about the site, so think about what someone searching for your site might search for and add those words/phrases here. 

##### Editing the Organizational branding variables

Edit the variables pictured below to replace the CDIL logo and link provided in the site header.  

{% include bootstrap/figure.md img="howto/orgbranding.png" caption="The Organization branding variables" alt="title line after editing" class="w-75" %}

Below is more on what these variables control

- `organization-name` --> This will adjust what shows up in the logo link's title and alt tags, for accessibility purposes.
- `organization-link` --> This is where a user where be taken if they click on the logo. 
- `organization-logo-banner` --> This is what logo will appear in the banner on larger screen widths. The image will appear on a white background. 
- `organization-logo-nav` --> This is what logo will appear on the navigation bar on screens with smaller widths (i.e. phones). The image will appear on a black background. 


## Step 4: Generate Your Site

{% include youtube/embed.html  video-id="ioubbjzQ9EY" title="Generate Your Site" display="d-none d-md-block" %}

- Go to the settings button at the top right of your repository page
{% include bootstrap/figure.md img="howto/settings_button.png" caption="" alt="settings button homepage of repository" %}
- Scroll down to the "GitHub Pages" section
- Change source dropdown button from "none" to "master" and copy the URL they give you. 
{% include bootstrap/figure.md img="howto/source_button.png" caption="" alt="picture of source drop down menu" class="w-50" %}
- It may take a couple minutes for the new website to build, depending on how big your site is. While your waiting, go back to the main page and click the "edit" button on your repository page
{% include bootstrap/figure.md img="howto/edit_button.png" caption="" alt="picture of the edit button above your repository" class="w-50" %}
- Add the copied url to the website section and click "save" 
{% include bootstrap/figure.md img="howto/url.png" caption="" alt="picture of save button" class="w-50" %}
- This will let you easily access the generated site whenever you come to edit the page. 
- Check out your new site by clicking on the link. Refresh if nothing shows up. Sometimes the GitHub service takes longer than others. 

***Congratulations on setting up your own oral history site!***

<a href="{{ 'howto/configurethesite.html' | relative_url }}" class='btn btn-lg btn-outline-primary m-2'>Previous Step: Configure your site</a>

<a href="{{ 'howto/prepareyourdata.html' | relative_url }}" class='btn btn-lg btn-outline-secondary m-2'>First Step: Prepare Your Data</a>
