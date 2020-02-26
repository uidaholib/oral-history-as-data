---
layout: page
title: About
order: 1
object-id: about
---
# Oral History as Data (OHD) - a Lib-STATIC Tool

The Oral History as Data (OHD) tool is a static website generator that allows users to analyze and publish coded oral history or qualitative interview files. By turning transcriptions into tagged/coded CSV files, adding a list of filters, and creating a simple markdown file for each interview (to be included in the _transcipt collection), OHD will provide filterable transcripts and a color coded visualization for all transcripts included. 

Use this site and the demo files included to learn how to use and deploy the code. Direct any questions here: 
<libstatic.uidaho@gmail.com>

Detailed How To instructions can be found here: 
{% include bootstrap/button.md text="Prepare Your Data" link="howto/prepareyourdata.html" color="info mb-2 text-left" %} 
{% include bootstrap/button.md text="Configure Your Site" link="howto/configurethesite.html" color="info" %}


---

{:.mt-4}
## Overview and Quick Start Instrucions

OHD will generate analyses, discovery and publication tools for oral histories and qualitative interviews, given three components:

- a CSV representation of the interview transcript(s), coded by cell 
    - [GitHub example](https://github.com/uidaholib/oral-history-as-data/blob/master/_data/transcripts/armantrout.csv){:target="_blank"}
    - [Google Sheet example](https://docs.google.com/spreadsheets/d/1PjPOTsLjGdfFyIn1S4UyzAWkSHjajCxE7kdxP6asQoE/edit?usp=sharing){:target="_blank"} 
- a folder (_transcripts) of markdown files for each transcript 
    - [MD file example](https://github.com/uidaholib/oral-history-as-data/edit/master/_transcripts/armantrout.md){:target="_blank"}
- If visualizations are wanted: a CSV list of coded topics, listing shorthand reference and full description 
    - [CSV Filters example](https://github.com/uidaholib/oral-history-as-data/blob/master/_data/filters.csv){:target="_blank"}

The tool uses the static website generator Jekyll with these components to then generate a website using GitHub Pages. 

### Quick Start Instructions
These instructions assume you will be doing most of the uploading through GitHub's web interface. If you'd like to do this on your computer, using Jekyll's built in development server, you'll need to install Jekyll (which requires Ruby). Instructions for installations can be found on the [CollectionBuilder Software page](https://collectionbuilder.github.io/docs/software.html) or on the [Lib-STATIC How-to pages](https://lib-static.github.io/howto/).

1. Go the [GitHub Repository for OHD](https://github.com/uidaholib/oral-history-as-data) and click the green "Use This Tempate" button.

2. Use the example [Google Sheets in this folder](https://drive.google.com/drive/folders/1Vkn6tWRow5-0z4ENJIf3vHWS-UDIQ5Z2?usp=sharing) and make copies of this blank [Google Sheet template](https://docs.google.com/spreadsheets/d/1uWrPMItiP-XOSkm7gyC8b9bl3tpSQRj9zLzS5y8QnW0/edit#gid=0) for all your interviews.

3. Fit your transcripts to the template/examples provided.

4. If you want subject-based visualizations, make sure your transcript sheet file is coded, using one-word abbreviations for your subjects in the "tags" column.

5. If you want to connect your transcripts with cloud based media files from youtube, vimeo, or soundcloud, make sure you have timestamps in the timestamps field like so: **[hh:mm:ss]**

5. Download each transcript as a Comma Separated Variable (CSV) file and add it to the `_data/transcripts` directory

6. Create a Markdown (.md) file for each interview you intend to include. Use the examples currently included in the _transcripts folder  as models.    
    - The minimum fields to be included at the top are: `object-id`  and `title`. 
    - `object-id` should match your CSV filename.

7. {:.mt-2}FOR VISUALIZATIONS: Revise the "filters.CSV" file in the `_data` directory to include your subjects/codes, including a shorthand for each topic in the 'shortfilter' column

8. Move the renamed CSV file(s) into the `_data/transcripts/` directory of your repository.
    - IMPORTANT: Your CSV file name must match the "object-id" variable in your Markdown file (next step) for this to work!!!
    - You can do this totally through the web interface if you'd like, just upload your CSVs to the `_data/transcripts` directory.

9. {:.mt-2}Edit the _config.yml file. 
    - Make sure that your github pages site (using your github username + ".github.io" as the website) is the `url` and your repository name is the `baseurl`. 

9. {:.mt-2}Go to your GitHub repository [Settings](/settings), and enable GitHub Pages (it's down the page a bit, so scroll).

10. Check out your new site by hitting the link that the enabled GH-Pages Settings sections provides. Should be something like: [GitHub Username].github.io/[Repository Name].

{%include credits.md%} 





