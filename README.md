# Oral History as Data (OHD) - a Lib-STATIC Tool

> **work in progress!**

The Oral History as Data (OHD) tool is a static website generator that allows users to analyze and publish coded oral history or qualitative interview files. By turning transcriptions into tagged/coded CSV files, adding a list of filters, and creating a simple markdown file for each interview (to be included in the _transcipt collection), OHD will provide filterable transcripts and a color coded visualization for all transcripts included. 

Use this site and the demo files included to learn how to use and deploy the code. Direct any questions here: 
<libstatic.uidaho@gmail.com>

# oral-history-as-data

<https://github.com/uidaholibrary/oral-history-as-data>

A project to generate analyses, discovery and publication tools for oral histories and qualitative interviews, given:

- a CSV representation of the interview transcript, coded by cell - CSV Transcript file example here
- a folder (_transcripts) markdown files for each transcript - MD file example here
- a CSV list of coded topics, listing shorthand reference and full description - CSV Filters example here

See [Getting Started Docs](docs/index.md) for detailed information (coming soon!).

### Get Started Quickly

### Get Started 

1. Fork or import this repository

2. Look at one of the csvs included in the _data directory of the repository
    - The CSVs included here are from the [CTRL+Shift project](www.ctrl-shift.org)
    - You can view them as Google Sheets as well: https://drive.google.com/drive/folders/1Vkn6tWRow5-0z4ENJIf3vHWS-UDIQ5Z2?usp=sharing

3. Make your transcript look like one of the examples
    - Paste your transcript into a google sheet or other spreadsheet software (WARNING: Excel sometimes adds artifacts (or changes data fomatting in unfortunate ways)
    
4. Make sure your sheet has these three header rows: speaker,words,tags
    - MAKE SURE THERE IS NO SPACE AFTER THE LAST HEADER FIELD (the tool won't read that field, if that's the case.)
    - If you don't want the visualization, and just need a searchable transcript online, you don't even need the tags!
    - (And, if that's the case, you don't even really need the speaker part either -- you could just paste the whole transcript into a sheet that breaks the paragraphs into cells and call the column "words")

6. If you do want visualizations, make sure your transcript sheet file is coded, using one-word abbreviations for your subjects in a colunm called "tags"
    - Code each cell/paragraph within the google sheet, dragging codes down for sections all about the same topic. For an example, see this [google sheet](https://docs.google.com/spreadsheets/d/1PjPOTsLjGdfFyIn1S4UyzAWkSHjajCxE7kdxP6asQoE/edit?usp=sharing) from an interview with Rae Armantrout

5.  Create a "filters.CSV" file in the _data directory (or just revise the one there already) to include your subjects/codes, including a shorthand for each topic in the 'shortfilter' column
    - For instance, in the example, we use the shorthand "paper" to represent the code we used to detail parts where our authors were talking about how they used paper. That row looks like this: (paper,using paper in the writing proceess)
    - See the example as a google sheet here: <https://docs.google.com/spreadsheets/d/1VtEdVgg__D3Gj3xwG9dgAieEv6pa-66iJTfaNYBgfHM/edit?usp=sharing>


7. Download your transcript file(s) from Google Sheets into a Comma Separated Variable format. 

8. Move the CSV file into the _data/transcripts/ directory of the repository you forked or imported (step 1).
    - you can do this totally through the web interface if you'd like
    - If you'd like to do this on your computer, using Jekyll's built in development server, you'll need to install Jekyll (which requires Ruby). Instructions for installations can be found on the [Lib-STATIC How-to pages](https://lib-static.github.io/howto/).

8. Create a Markdown (.md) file for each interview CSV file you intend to include. Use the examples currently included as models. The minimum fields to be included at the top are: object-id  and title. You can also add 'date-interviewed', 'location', and 'interviewer'. 

9. If you're working on the web, go to your GitHub repository [Settings](/settings), and enable GitHub Pages.

10. Check out your new site by hitting the link that the enabled GH-Pages Settings sections provides. Should be something like: [GitHub Username].github.io/[Repository Name].

## Features

- [Jekyll](https://jekyllrb.com/) for GitHub Pages 
- Layout using [Bootstrap](https://getbootstrap.com/docs/4.0/getting-started/introduction/).
- [jQuery](https://jquery.com/)
- Simple [lunr](https://lunrjs.com/) search (this isn't really working right now ...)
- Rich markup using [Schema.org](http://schema.org) and [Open Graph protocol](http://ogp.me/) standards.






