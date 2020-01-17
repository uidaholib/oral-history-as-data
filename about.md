---
layout: page
title: About
order: 1
object-id: about
---
# Oral History as Data (OHD) - a Lib-STATIC Tool

> **work in progress!**

The Oral History as Data (OHD) tool is a static website generator that allows users to analyze and publish coded oral history or qualitative interview files. By turning transcriptions into tagged/coded CSV files, adding a list of filters, and creating a simple markdown file for each interview (to be included in the _transcipt collection), OHD will provide filterable transcripts and a color coded visualization for all transcripts included. 

Use this site and the demo files included to learn how to use and deploy the code. Direct any questions here: 
<libstatic.uidaho@gmail.com>

# oral-history-as-data

<https://github.com/uidaholib/oral-history-as-data>

A project to generate analyses, discovery and publication tools for oral histories and qualitative interviews, given:

- a CSV representation of the interview transcript, coded by cell - CSV Transcript file example here
- a folder (_transcripts) markdown files for each transcript - MD file example here
- a CSV list of coded topics, listing shorthand reference and full description - CSV Filters example here


### Get Started 

1. Fork or import this repository
2. Look at one of the csvs included (CSVs included here are from the [CTRL+Shift project](www.ctrl-shift.org)
3. Paste your transcript into a google sheet or other spreadsheet software (Excel adds artifacts that can interfere with Jekyll)
4. Make sure you have these rows at minimum: speaker,words,tags
5. Revise the _data/filters.csv to include your subjects/codes, including a shorthand for each topic in the 'shortfilter' column
6. If you haven't added subject coding to your transcript CSV file, do so, using the shortfilter words you used in the filters.csv
7. Download your file as into a CSV format. Add the csv file in the _data/transcripts/ directory.
8. Create a Markdown (.md) file for each interview CSV file you intend to include. Use the examples currently included as models. The minimum fields to be included at the top are: object-id, first-name, last-name. If you can, add: last-name, date-interviewed, location, interviewer. 
9. If you're working on the web, go to your GitHub repository [Settings](/settings), and enable GitHub Pages
10. Check out your new site by hitting the link that the enabled GH-Pages Settings sections provides. Should be something like: [GitHub Username].github.io/[Repository Name].

{%include credits.md%} 





