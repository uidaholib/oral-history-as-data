---
layout: howto
title: How To Edit Your _config.yml Folder
---

When you design your website you'll need to utilize the *_config.yml* folder to help establish the working parameters of your page, the basic information that inhabits it, and the general layout your visitors interact with. 

{:.alert .alert-warning .mb-4}
NOTE: when you are navigating through this folder, you will notice hashtags which denote useful information about how various lines effect your page. 

### Step 1: Get into the *_config.yml folder* 
- First, we're going to find the *_config.yml* folder. You'll find this on the main page of your site's repository. Click on this folder and open it up.  
{% include bootstrap/figure.md img="howto/configscreen.png" caption="image of _config.yml folder found on main page of repository" alt="image of config folder" class="w-50" %}

- Once you open up the folder, you'll need to enable editing. You're going to see a pencil icon at the top, right corner of the page. Click on this to enable editing. 
{% include bootstrap/figure.md img="howto/edit_pencil.png" caption="" alt="image of config folder" class="w-50" %}

### Step 2: Editing your *url, baseurl*, and *repository* (URL settings)

- First, you'll need to change your url. To do this, delete "uidaholib" from the *url* line, and replace it with your GitHub username. 
{% include bootstrap/figure.md img="howto/beforename.png" caption="url before edit" alt="url line in config folder before being edited" class="w-50" %}

{% include bootstrap/figure.md img="howto/aftername.png" caption="url after edit" alt="url line after editing" class="w-50" %}

- Now you'll need to edit your *baseurl*. After the forward slash you'll delete "oral-history-as-data" and type the name of your repository. 
{% include bootstrap/figure.md img="howto/basebefore.png" caption="baseurl line before edit" alt="image of baseurl line before edit" class="w-50" %}
{% include bootstrap/figure.md img="howto/baseafter.png" caption="baseurl line after edit" alt="image of baseurl line after edit" class="w-50" %}

- Finally, we'll edit your *repository* line. You're going to erase the text that reads "uidaholib" and replace it with your username. Then you're going to take the final piece of the line that reads "oral-history-as-data" and replace it with your repository name. 

{% include bootstrap/figure.md img="howto/beforerepos.png" caption="repository before edit" alt="repository line before editing" class="w-50" %}
{% include bootstrap/figure.md img="howto/afterrepos.png" caption="repository after edit" alt="repository line after editing" class="w-50" %}

### Step 3: Editing *title, tagline,* *and description* (site settings)

- Now scroll down to the next section in this folder titled *site settings*. Go to the first line called *title* and change "Oral History (as) Data" to what ever you would like to call your site. 
{% include bootstrap/figure.md img="howto/beforetitle.png" caption="title before edit" alt="title line before editing" class="w-50" %} 

{% include bootstrap/figure.md img="howto/aftertitle.png" caption="title after edit" alt="title line after editing" class="w-50" %}

- Now we're going to edit the *tag line*, which is a short banner that will run across your site next to the title. You're going to replace the text next to *tagline* that says "analyze and publish coded oral history and qualitative interviews" with whatever site description you would like. 
{% include bootstrap/figure.md img="howto/beforetag.png" caption="tagline before edit" alt="tagline before editing" class="w-50" %}

{% include bootstrap/figure.md img="howto/aftertag.png" caption=" tagline after edit" alt="title line after editing" class="w-50" %}

## Step 4: Generate Your Site

- Go to the settings button at the top right of your repository page
{% include bootstrap/figure.md img="howto/settings_button.png" caption="" alt="settings button homepage of repository" %}
- Scroll down to the "GitHub Pages" section
- Change source dropdown button from "none" to "master" and copy the URL they give you. 
{% include bootstrap/figure.md img="howto/source_button.png" caption="" alt="picture of source drop down menu" class="w-50" %}
- It will take several minutes for the new website to build, while your waiting go back to the main page and click the "edit" button on your repository page
{% include bootstrap/figure.md img="howto/edit_button.png" caption="" alt="picture of the edit button above your repository" class="w-50" %}
- Add the copied url to the website section and click "save" 
{% include bootstrap/figure.md img="howto/url.png" caption="" alt="picture of save button" class="w-50" %}
- This will let you easily access the generated site whenever you come to edit the page. 
- Check out your new site by clicking on the link. Refresh if nothing shows up. Congratulations on setting up your own oral history site!



### Optional: AV settings 

{:.alert .alert-info}
OHD has the option of linking an audio or video file to your transcript, to enhance the experience for the user. It is compatible with YouTube, Vimeo, and Soundcloud. 

- First, you'll need to look at the *av_source* line. You'll see that there are a list of options: "YouTube, Vimeo, Soundcloud". OHD has YouTube set as the default option. But if you wish to choose a different option you can easily change it by erasing YouTube and writing either Soundcloud or Vimeo.
{% include bootstrap/figure.md img="howto/youtube.png" caption=" av_source line with default YouTube selection" alt="picture of the av_source line in folder" class="w-50" %}


- If you are using Soundcloud, you will need to include your Soundcloud ID, which can be found in the url of your Soundcloud files.  
{% include bootstrap/figure.md img="howto/soundcloud_copy.png" caption=" unedited soundcloud-id section with circle indicating where to find soundcloud id" alt="picture of soundcloud-id line with circle indicating where to find a soundcloud id on soundcloud's website" class="w-50" %}

{% include bootstrap/figure.md img="howto/soundcloud2.png" caption="example text indicating where to place Soundcloud ID" alt="title line after editing" class="w-50" %}

