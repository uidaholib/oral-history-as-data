---
layout: howto
title: How To Prepare Your Data
---
{% include youtube/playlist.html playlist-id="PL_71zYZtmyTsCNq2jnacVmCf0L2Gt-YyC" title="Prepare your Data Playlist of All Included Videos" display="d-block d-md-none" %}

{% include youtube/embed.html video-id="0LLE_FXKs64" title="Make a Copy of the Template Spreadsheet" display="d-none d-md-block" %}

For OHD to work with your transcript or other data, you will need to transform your transcripts/data into CSV files. Below are a few steps to help you properly prepare your transcripts for compatible use with Oral Histories As Data.  

## Step 1: Set up Your Spreadsheet

- Here is a [template](https://docs.google.com/spreadsheets/d/1uWrPMItiP-XOSkm7gyC8b9bl3tpSQRj9zLzS5y8QnW0/edit?usp=sharing){:target="_blank"} to help you get started. 
- Make a copy of the template by going to the "file" tab at the top and selecting "make a copy". 
- Give your transcript a simple name. 


## Step 2: Clean Your Transcript and Paste It Into your Spreadsheet

{% include youtube/embed.html  video-id="5Bun9Ttr00U " title="Steps 2 and 3 <br> Clean Text and Edit Tags" display="d-none d-md-block" %}

Smart quotes, signal character ellipses, and other artifacts won't render correctly on the web so it's best to clean your text before you transform it for the tool. To do so: 

- Take the text from your transcript (be that in a Word file, a PDF or some other format) and run it through this [text cleaner provided by Jonathan Hedley](https://jhy.io/tools/convert-word-to-plain-text){:target="_blank"}
    - This should also make it so that your transcript transfers nicely into the cells of your spreadsheet.   
- Copy and paste the text into the top window, press clean, and then copy the text from the bottom window. 

{% include bootstrap/figure.md img="howto/text_cleaner_2.png" caption="" alt="a screenshot of the first section of the text cleaner web page" class="w-50" %}

- Paste the clean text you made in Step 1 into the Google Sheet you made in step 1. Be sure to paste it just below the cell titled "speaker".  

{% include bootstrap/figure.md img="howto/speaker_copy.png" caption="copy text here" alt="picture of correct cell placement for pasting transcript" class="w-50" %}

## Step 3: Add Tags/Codes to Your Transcript Spreadsheet (Optional)

*Note: in order to enable the visualization, you must have coded your spreadsheet*

If you'd like to enable subject-based browsing and color-coded visualizations for you transcript, you need to "code" portions of the conversation according to the subject matter. 

- To do this, start adding "tags"-- which should be shorthand descriptions of larger thematic subjects that pertain to this and other transcripts in a collect-- in the cells under the "tags" column that pertain to the content in the adjacent "words" cell. 
{% include bootstrap/figure.md img="howto/subjects_cell.png" caption="example subjects" alt="picture of the subjects cells" %}
- If you have multiple subjects in a cell, separate them with a semi-colon (as pictured above). 
- You'll often want to cover a large portion of the transcript with the same tags. In Google Sheets, you can do this by hovering over the bottom right of a cell (pictured below) and then dragging your cursor across the pertinent sections of the transcript below or above where you started. 
    - This saves a great deal of time, as usually sections of the oral history are all pertaining to the same tags/subjects. 
{% include bootstrap/figure.md img="howto/bottom-right-corner.png" caption="Click here, hold, and drag the cursor down to pull down the tags across a section " alt="image of example subjects in cells" %}

{:.alert .alert-info .col-md-8} 
**See a finished transcript:** You can check out what a finished transcript look like in this [Sample Google Sheet](https://docs.google.com/spreadsheets/d/1PjPOTsLjGdfFyIn1S4UyzAWkSHjajCxE7kdxP6asQoE/edit?usp=sharing){:target="_blank"}

## Step 4: Download Your Transcript Spreadsheet as a CSV

{% include youtube/embed.html  video-id="FAQmA-RWCvQ " title="Downloading Transcript as CSV" display="d-none d-md-block" %}
- Once you've edited the Google Sheet and gotten everything in order, go to the "file" tab at the top of your sheet and hover over "download"
- Select "comma-separated values"  to save your file as a .csv file
- Once downloaded, rename your transcript so that's its as simple as possible, removing any spaces or special characters. 
    - We typically use either just the last name, for small collections, or `lastname_firstname`, for larger collections. Make sure the file retains its (.csv) extension.
{% include bootstrap/figure.md img="howto/creating_csv_final.png" caption="" alt="picture of the dropdown option for creating a csv sheet" class="w-50" %}

{% include youtube/embed.html  video-id="emeMzhGP5mQ" title="Edit Filters csv" display="d-none d-md-block" %}

## Step 5: Create Your Filters.CSV (optional)

The filters.csv file will communicate with the tags you enter into the the `tags` field of your transcript's CSV to create the tool's color-coded visualizations (seen below). 

{:.clearfix}
{% include bootstrap/figure.md img="howto/wrigley-viz.png" caption="Picture of visualization created through filters.csv" alt="A visualization of Robert Wrigley's transcript, as enabled by the Filters.CSV" class="border-0 w-50" link="/oral-history-as-data/subjects.html?id=wrigley" %}


- Open this blank [spreadsheet](https://docs.google.com/spreadsheets/d/1qPU-7LFZrIWcLiHuTqnlbnRD1869SJalJ5OCL7tGtzE/edit#gid=0){:target="_blank"}. 
- Click the "file" icon and choose "make a copy." 
- In the "tag" column write out the tags you wish to include in the transcript.
- In the "description" column write out a brief description of that tag. 
- When you're finished create a new .csv by clicking on the "file" icon, hovering above "download", and selecting "comma-separated values". 
- Rename this file: `filters.csv`




