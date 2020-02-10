---
layout: howto
title: How To Configure the Website
---

Below are a few quick steps to help you begin configuring your GitHub site for use with Oral Histories as Data (OHD). 

## Step 1: Make a Template of OHD

- Go to the OHD homepage and click on the "Template" button toward the top right of the page. 
{% include bootstrap/figure.md img="howto/ohd_template.png" caption="" alt="" class="w-50" %}
- You'll need to then name your repository.
{% include bootstrap/figure.md img="howto/name_repository.png" caption="" alt="" class="w-50" %}
- Once you've named your repository you'll need to click the "Create Repository From Template" button. 
{% include bootstrap/figure.md img="howto/create_repository_button.png" caption="" alt="" class="w-50" %}

## Step 2: Create a New File

- Now you'll need to go into you "data" folder and then into the "transcripts" folder in your repository. 
- Once in transcripts click on "create new file".  
{% include bootstrap/figure.md img="howto/new_file.png" caption="" alt="" class="w-50" %}
- Now you need to name your file according to your transcript. 
{% include bootstrap/figure.md img="howto/name_file.png" caption="" alt="" class="w-50" %}

{:.alert .alert-danger}
When you name your file be sure to include the type of file after the name you choose. For example, if it is a mark down file, attach ".md" after the file name. 
- Once you've named the file scroll to the bottom of the page and click "commit new file". 
{% include bootstrap/figure.md img="howto/commit_file.png" caption="" alt="" class="w-50" %}

## Step 3: Moving Transcript

- Open your transcript  

{:.alert .alert-danger}
Make sure you open your transcript in a text editor. Here at OHD, we prefer using Visual Studio Code, but a list of other options are available. 
- Move the transcript to the new GitHub file by opening it in the text editor, select the entire text (ctrl + a), then copy and paste it into the new file open you have created.
{% include bootstrap/figure.md img="howto/text_editor.png" caption="transcript selected in text editor" alt="" class="w-50" %}
{% include bootstrap/figure.md img="howto/github_csv.png" caption=".csv after being transferred to GitHub" alt="" class="w-50" %}
- Commit the change at bottom of page 

#### Additional: Moving filters.csv
OHD offers a way to categorize your transcripts using tags. This is done through two locations: the subject cells in your transcript's .csv and the filters.csv file, which is already provided for you in the structure of OHD. If you are not aware of either of these files, first visit our steps on "How To Prepare Your Data." 

- Open filters.csv you created
- navigate to the "_data" folder 
- Open the "_data" folder and click the pencil icon to edit 
- Copy and paste this filters.csv over over the existing content 
{% include bootstrap/figure.md img="howto/filters_csv2.png" caption="transcript selected in text editor" alt="" class="w-50" %}
{% include bootstrap/figure.md img="howto/filters_github.png" caption=".csv after being transferred to GitHub" alt="" class="w-50" %}
- Commit the change at the bottom of the page 
- Your finished visualization will look like this: 
{% include bootstrap/figure.md img="howto/visualization.png" caption="finished OHD visual" alt="" class="w-50" %}

## Generate Your Site

- Go to the settings button at the top right of your repository page
{% include bootstrap/figure.md img="howto/settings_button.png" caption="" alt="settings button homepage of repository" %}
- Scroll down to the "GitHub Pages" section
- Change source dropdown button from "none" to "master" and copy the URL they give you. 
{% include bootstrap/figure.md img="howto/source_button.png" caption="" alt="" class="w-50" %}
- Go back to the main page and click the "edit" button on your repository page
{% include bootstrap/figure.md img="howto/edit_button.png" caption="" alt="" class="w-50" %}
- Add the copied url to the website section and click "save" 
{% include bootstrap/figure.md img="howto/url.png" caption="" alt="" class="w-50" %}


