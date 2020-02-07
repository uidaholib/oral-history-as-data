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
- Once you've named the file scroll to the bottom of the page and click "commit new file". 
{% include bootstrap/figure.md img="howto/commit_file.png" caption="" alt="" class="w-50" %}

## Step 3: Moving Transcript

- Open your transcript  
- Make sure you open it in a text editor. 
- Move the transcript to the new GitHub file by opening it in the text editor, select the entire text (ctrl + a), then copy and paste it into the new file open you have created.
{% include bootstrap/figure.md img="howto/text_editor.png" caption="transcript selected in text editor" alt="" class="w-50" %}
{% include bootstrap/figure.md img="howto/github_csv.png" caption=".csv after being transferred to GitHub" alt="" class="w-50" %}
- Commit the change at bottom oof page 

## Step 4: Moving filters.csv

- Open filters.csv you created
- navigate to the "_data" folder 
- Open the "_data" folder and click the pencil icon to edit 
- Copy and paste this filters.csv over over the existing content 
{% include bootstrap/figure.md img="howto/filters_csv2.png" caption="transcript selected in text editor" alt="" class="w-50" %}
{% include bootstrap/figure.md img="howto/filters_github.png" caption=".csv after being transferred to GitHub" alt="" class="w-50" %}
- Commit the change at the bottom of the page 

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


