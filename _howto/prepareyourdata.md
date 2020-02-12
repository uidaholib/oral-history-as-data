---
layout: howto
title: How To Prepare Your Data
---

Below are a few simple steps to help you properly prepare your transcripts for compatible use with Oral Histories As Data.

## Step 1: Setting up Your Spreadsheet

- Here is a [template](https://docs.google.com/spreadsheets/d/1uWrPMItiP-XOSkm7gyC8b9bl3tpSQRj9zLzS5y8QnW0/edit?usp=sharing){:target="_blank"} to help you get started. 
- Before you copy and paste your text into the spreadsheet, you'll need to make a copy of it. Go to the "file" tab at the top and select "make a copy". 
- Now take the text from your transcript (be that in a Word file, a PDF or some other format) and run it through this [text cleaner provided by Jonathan Hedley](https://jhy.io/tools/convert-word-to-plain-text){:target="_blank"}  
- Copy and paste the text into the top window, press clean, and then copy the text from the bottom window. 
{% include bootstrap/figure.md img="howto/text_cleaner_2.png" caption="" alt="a screenshot of the first section of the Ruby Installer website" class="w-50" %}
- Paste the text into the "copy" of the starter transcript spreadsheet you made above. Be sure to paste it just below the cell titled "speaker".  
{% include bootstrap/figure.md img="howto/speaker_copy.png" caption="copy text here" alt="picture of correct cell placement for pasting transcript" class="w-50" %}

{:.alert .alert-warning} 
At this point you may need to use your skills to clean up this data. The main thing to focus on is getting the actual transcript into the "words" column. The tool will work even if that's the only column filled. Also, feel free to view our video tutorial on cleaning up .csv data for some helpful tips.
- Now you will need to "code" your transcript. This can be done by adding "tags"--which should be shorthand descriptions of larger thematic subjects that pertain to this and other transcripts--in the cells under the "tags" column.
{% include bootstrap/figure.md img="howto/subjects_cell.png" caption="example subjects" alt="picture of the subjects cells" %}
- Note, if you have multiple subjects in a cell you will need to separate them using a semi-colon with no space (as pictured above). 
- You can also hover over the bottom right of a cell (pictured below) and then drag the tags you entered across sections of the transcript. This helps a good deal, as usually sections of the oral history are all pertaining to the same tags/subjects. 
{% include bootstrap/figure.md img="howto/bottom-right-corner.png" caption="Click here, hold, and drag the cursor down to pull down the tags across a section " alt="image of example subjects in cells" %}


## Step 2: Transforming Your Transcript Into a .CSV

- Once you've edited the Google Sheet and gotten everything in order, go to the "file" tab at the top of your sheet and hover over "download"
- Select "comma-separated values"  to save your file as a .csv file
{% include bootstrap/figure.md img="howto/creating_csv_final.png" caption="" alt="picture of the dropdown option for creating a csv sheet" class="w-50" %}

## Step 3: Creating Your "filters.csv" 

{:.alert .alert-info}
The filters.csv will communicate with the tags you enter into the your transcript's .csv. The result will be an interactive element of OHD, comprised of a visualization and the ability to broaden and limit user focus when reading provided transcripts. Below is an image of a completed OHD visualization and a list of quick steps to help you set up your own "transcripts.csv". 
- First, go to this blank [spreadsheet](https://docs.google.com/spreadsheets/d/1qPU-7LFZrIWcLiHuTqnlbnRD1869SJalJ5OCL7tGtzE/edit#gid=0){:target="_blank"}. 
- Click the "file" icon and choose "make a copy." 
- In the "tag" column write out the tags you wish to include in the transcript.
- In the "description" column write out a brief description of that tag. 
- Finally, you create a new .csv by clicking on the "file" icon, hovering above "download", and selecting "comma-separated values". 