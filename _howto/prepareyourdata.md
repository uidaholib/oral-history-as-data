---
layout: howto
title: How To Prepare Your Data
---
{% include youtube/playlist.html playlist-id="PL_71zYZtmyTsCNq2jnacVmCf0L2Gt-YyC" title="Prepare your Data Playlist of All Included Videos" display="d-block d-sm-none" %}

For OHD to work with your transcripts, you will need to transform your transcripts into CSV files.
<<<<<<< HEAD
Below are a few simple steps to help you properly prepare your transcripts for compatible use with Oral Histories As 
Data.  

{% include youtube/embed.html video-id="0LLE_FXKs64" title="Make a Copy of the Template Spreadsheet" display="d-none d-md-block" %}
## Step 1: Set up Your Spreadsheet

- Use this [template](https://docs.google.com/spreadsheets/d/1uWrPMItiP-XOSkm7gyC8b9bl3tpSQRj9zLzS5y8QnW0/edit?usp=sharing){:target="_blank"} to get started. 

- Make a copy of the template by going to the "file" tab at the top and selecting "make a copy". 

{:.alert .alert-warning .col-md-8} 
At this point you may need to use your skills to clean up this data. The main thing to focus on is getting the actual transcript into the "words" column. The tool will work even if that's the only column filled. 

{% include youtube/embed.html  video-id="5Bun9Ttr00U " title="Clean Text and Edit Tags" display="d-none d-md-block" %}

## Step 2: Clean Your Transcript and Add Tags/Codes to Your Transcript Spreadsheet

- Now take the text from your transcript (be that in a Word file, a PDF or some other format) and run it through this [text cleaner provided by Jonathan Hedley](https://jhy.io/tools/convert-word-to-plain-text){:target="_blank"}  
- Copy and paste the text into the top window, press clean, and then copy the text from the bottom window. 

{% include bootstrap/figure.md img="howto/text_cleaner_2.png" caption="" alt="a screenshot of the first section of the text cleaner web page" class="w-50" %}

- Paste the clean text you made in Step 1 into the "copy"of the starter transcript spreadsheet you made above. Be sure to paste it just below the cell titled "speaker".  

{% include bootstrap/figure.md img="howto/speaker_copy.png" caption="copy text here" alt="picture of correct cell placement for pasting transcript" class="w-50" %}
- Now you will need to "code" your transcript. This can be done by adding "tags"--which should be shorthand descriptions of larger thematic subjects that pertain to this and other transcripts--in the cells under the "tags" column.
{% include bootstrap/figure.md img="howto/subjects_cell.png" caption="example subjects" alt="picture of the subjects cells" %}
- Note, if you have multiple subjects in a cell you will need to separate them using a semi-colon with no space (as pictured above). 
- You can also hover over the bottom right of a cell (pictured below) and then drag the tags you entered across sections of the transcript. This helps a good deal, as usually sections of the oral history are all pertaining to the same tags/subjects. 
{% include bootstrap/figure.md img="howto/bottom-right-corner.png" caption="Click here, hold, and drag the cursor down to pull down the tags across a section " alt="image of example subjects in cells" %}

## Step 3: Download Your Transcript Spreadsheet as a CSV

{% include youtube/embed.html  video-id="FAQmA-RWCvQ " title="Downloading Transcript as CSV" display="d-none d-md-block" %}
- Once you've edited the Google Sheet and gotten everything in order, go to the "file" tab at the top of your sheet and hover over "download"
- Select "comma-separated values"  to save your file as a .csv file
{% include bootstrap/figure.md img="howto/creating_csv_final.png" caption="" alt="picture of the dropdown option for creating a csv sheet" class="w-50" %}

{% include youtube/embed.html  video-id="emeMzhGP5mQ" title="Edit Filters csv" display="d-none d-md-block" %}
## Step 4: Create Your Filters.CSV 
The filters.csv file will communicate with the tags you enter into the the `tags` field of your transcript's CSV to create an interactive visualization of the codes used in your transcripts.  Below is an image of a list of quick steps to help you set up your own "transcripts.csv" and a completed OHD [visualization]({{ '/visualizations.html?id=wrigley' | relative_url }}). 

- First, go to this blank [spreadsheet](https://docs.google.com/spreadsheets/d/1qPU-7LFZrIWcLiHuTqnlbnRD1869SJalJ5OCL7tGtzE/edit#gid=0){:target="_blank"}. 
- Click the "file" icon and choose "make a copy." 
- In the "tag" column write out the tags you wish to include in the transcript.
- In the "description" column write out a brief description of that tag. 
- Finally, you create a new .csv by clicking on the "file" icon, hovering above "download", and selecting "comma-separated values". 

{:.clearfix}
{% include bootstrap/figure.md img="howto/wrigley-viz.png" caption="Picture of visualization created through filters.csv" alt="A visualization of Robert Wrigley's transcript, as enabled by the Filters.CSV" class="border-0" %}

