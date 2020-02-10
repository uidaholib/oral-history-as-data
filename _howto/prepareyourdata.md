---
layout: howto
title: How To Prepare Your Data
---

Below are a few simple steps to help you properly prepare your transcripts for compatible use with Oral Histories As Data.

## Step 1: Setting up Your Spreadsheet

- Here is a [template](https://docs.google.com/spreadsheets/d/1uWrPMItiP-XOSkm7gyC8b9bl3tpSQRj9zLzS5y8QnW0/edit?usp=sharing){:target="_blank"} to help you get started. 
- Before you copy and paste your text into the spreadsheet, you'll need to make a copy of it. Go to the "file" tab at the top and select "make a copy". 
- Now take the text from your word file and run it through this text [cleaner](https://jhy.io/tools/convert-word-to-plain-text){:target="_blank"}  
- Copy and paste the text into the top window, press clean, and then copy and paste the text from the bottom window into your spreadsheet. 
{% include bootstrap/figure.md img="howto/text_cleaner_2.png" caption="" alt="a screenshot of the first section of the Ruby Installer website" class="w-50" %}
- when you copy the text into your spreadsheet be sure to copy it just below the cell titled "speaker".  
{% include bootstrap/figure.md img="howto/speaker_copy.png" caption="copy text here" alt="a screenshot of the first section of the Ruby Installer website" class="w-50" %}

{:.alert .alert-danger} 
At this point you may need to use your skills to clean up this data. But if you are having a difficult time feel free to view our video tutorial on cleaning up .csv data. 
- Now add subjects in the cells under the "tags" column.
{% include bootstrap/figure.md img="howto/subjects_cell.png" caption="example subjects" alt="a screenshot of the first section of the Ruby Installer website" %}
- Note, if you have multiple subjects in a cell you will need to separate them using a semi-colon with no space. 

## Step 2: Transforming Your Transcript Into a .CSV

- Go to the "file" tab at the top of your sheet and hover over "download"
- Select "comma-separated values"  to save your file as a .csv file
{% include bootstrap/figure.md img="howto/creating_csv_final.png" caption="" alt="a screenshot of the first section of the Ruby Installer website" class="w-50" %}

## Step 3: Creating Your "filters.csv" 

{:.alert .alert-info}
The filters.csv will communicate with the tags you enter into the your transcript's .csv. The result will be an interactive element of OHD, comprised of a visualization and the ability to broaden and limit user focus when reading provided transcripts. Below is an image of a completed OHD visualization and a list of quick steps to help you set up your own "transcripts.csv". 
- First, go to this blank [spreadsheet](https://docs.google.com/spreadsheets/d/1qPU-7LFZrIWcLiHuTqnlbnRD1869SJalJ5OCL7tGtzE/edit#gid=0){:target="_blank"}. 
- Click the "file" icon and choose "make a copy." 
- Under shortfilter write out the tags you wish to include in the transcript.
- Under text write out a brief description of that tag. 
- Finally, you create a new .csv by clicking on the "file" icon, hovering above "download", and selecting "comma-separated values". 