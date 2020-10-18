---
layout: howto
title: How To Configure Your Website
---

Below are a few quick steps to help you begin configuring your GitHub site for use with Oral Histories as Data (OHD). 

{% include youtube/embed.html  video-id="lJ9b0VNJIMw" title="Making a Filter" display="d-none d-md-block" %}
## Step 1: Make a Template of OHD

- Go to the OHD homepage and click on the green "Use this template" button toward the top right of the page. 

{% include bootstrap/figure.md img="howto/ohd_template.png" caption="" alt="picture of the button that enables user to create a new template in github" class="w-50" %}

- Name your repository.
{% include bootstrap/figure.md img="howto/name_repository.png" caption="" alt="image of the field users must fill out in order to create a name for their new template" class="w-50" %}

- Click the "Create Repository From Template" button -- this will copy all the files (but not the history!) of the Oral History as Data repository into your own repository. 
{% include bootstrap/figure.md img="howto/create_repository_button.png" caption="" alt="picture of the create repository button located at the bottom of the page" class="w-50" %}

## Step 2: Upload Your Transcript

- Click on the `_data` folder, which will take you to a new page. 
- Then click into the `transcripts` folder.   
- Once you're in the transcripts folder, find the transcript spreadsheet/CSV file or files you've created in your Finder or File Explorer. 
    - Make sure the transcript CSV is titled something simple, and that it's all lowercase and has no spaces or special characters. E.G. `doe_john.csv` (And make sure it has a `.csv` extension!)
- Drag the file or files onto the web page -- the page will change when you drag it onto the webpage to say "Drop to Upload Your Files". Drop the file to upload it!
    - Alternatively, you can push the "Add File" dropdown button at the top right of your screen, and then select the file(s) you'd like to upload.
- Once it's uploaded, you'll need to commit your change to make it permanent. Commit your upload at bottom of page by scrolling to the bottom of the page and clicking "commit new file". 
{% include bootstrap/figure.md img="howto/commit_file.png" caption="" alt="" class="w-50" %}
- Below is what the CSV should look like after you've committed it into your GitHub repository. 
{% include bootstrap/figure.md img="howto/github_csv.png" caption="This is how the CSV should look after you paste it into the new file and commit it." alt="complete and committed csv in github" class="w-50" %}


{:.alert .alert-warning .mb-4}
NOTE: If the CSV has a problem, GitHub will show you an error message that will say: "We can make this file beautiful and searchable if this error is corrected:" After that phrase, they will also point out a line number that is causing the problem. Open the file up by clicking on the pencil icon in the top right of the file area. Go to the line indicated and see if there's an obvious error. If you can't get it fixed, go back to your Google Sheet and see if there's anything to clean up. Even if there is nothing wrong, re-download the file as a CSV, rename it to the new title, then drag it back to the page as you did above. Hopefully one of these steps clears up the problem. 

{% include youtube/embed.html  video-id="kfDeEfjl6nQ" title="Creating a .MD File" display="d-none d-md-block" %}
## Step 4: Creating a Markdown File

- Navigate back to the root of your repository by clicking on `<> Code ` at the top left of the page.
- Click on the folder that says "_transcripts" 
{% include bootstrap/figure.md img="howto/transcripts.png" caption="" alt="_transcipts button" class="w-50" %}
- Open up any of the .md file examples that are in this folder
- Navigate to the button that says "raw" and click it
{% include bootstrap/figure.md img="howto/raw.png" caption="" alt="raw file button" class="w-50" %}
- Copy the text inside of the file you opened
{% include bootstrap/figure.md img="howto/newcopyandpaste.png" caption="" alt="raw file text" class="w-50" %}
- Go back to your _transcripts directory by clicking back two pages in your browser.
- Click the "Create New File" button
{% include bootstrap/figure.md img="howto/createnewmd.png" caption="" alt="create new file button" class="w-50" %}
- Name this file the same name you named your transcript file, but be sure to put `.md `rather than `.csv`, as it's extension.  

{% include bootstrap/figure.md img="howto/mdname.png" caption="" alt="name field in new markdown file" class="w-50" %}

{:.alert .alert-info .mb-4}
You are creating a markdown file; [more on Markdown here](https://www.markdownguide.org/). 
Jekyll uses the markdown file as the basis for creating web pages. All the information stored between the two `---` at the top and then down a bit is called frontmatter. This frontmatter is written in a language called YAML, which is a [a human-readable language for writing/storing data variables](https://en.wikipedia.org/wiki/YAML). (You'll work with some `.yml` files later as well)

- Paste the text you copied from the raw file you opened earlier into this new file.
{% include bootstrap/figure.md img="howto/beforemd1.png" caption="Pasted text before editing" alt="pasted text in new .md file" class="w-50" %}
- Edit the variables in the frontmatter between the `---` lines ) to fit your data -- be sure that the object-id option is the same as the filename (without the extension) of your transcript. 
{% include bootstrap/figure.md img="howto/aftermd2.png" caption="File after being edited for new file" alt="new .md file text after being edited for new file" class="w-50" %}

{:.alert .alert-warning .mb-4}
NOTE: if the "object-id" field is different than the name of your transcript CSV file in the _data/transcripts folder, the tool will not work. The transcript file will have an extension (.csv) but the object-id should not have an extension. So if the transcript is called `doe_john.csv`, then the object-id for the corresponding Markdown file should be `doe_john`.

- Write a commit message, briefly describing the changes you made and then commit them at the bottom.
- Once you are done, navigate to your new file, it should look like the example below
{% include bootstrap/figure.md img="howto/comletemd.png" caption="" alt="the newly created md file" class="w-50" %}

### Optional: adding an audio or video file using av_source

{:.alert .alert-info}
You may want to include an auditory or visual component to your transcript. You'll need to incorporate some simple information in the header of your markdown file. By including a video or audio file, you can correspond recorded dialogue to your written transcript. 

- Look in the header of your markdown file. You'll see that there is a space for av_source. Here you have four options, using OHD: `mp3, youtube,  soundcloud, or vimeo`. 

Using all lowercase letters, type the platform's name where your file is uploaded. 
{% include bootstrap/figure.md img="howto/avid1.png" caption="" alt="opened file, ready for editing" class="w-50" %}
- Below av_source, you'll see a space for your file's audiovideo-id. Fill in this information. 
{% include bootstrap/figure.md img="howto/avid2.png" caption="" alt="opened file, ready for editing" class="w-50" %}
- Below are pictures indicating the location of various audiovideo-id locations on different platforms. 
{% include bootstrap/figure.md img="howto/youtubeid.png" caption="location of your youtube audiovideo-id" alt="opened file, ready for editing" class="w-50" %}
{% include bootstrap/figure.md img="howto/vimeoid2.png" caption="location of your vimeo audiovideo-id" alt="opened file, ready for editing" class="w-50" %}
{% include bootstrap/figure.md img="howto/soundcloud_path_copy.png" caption="location of your the URL path" alt="opened file, ready for editing" class="w-50" %}


{:.alert .alert-warning .mb-4}
NOTE: if you want to utilize an mp3 file, you can create also create a webpage to house your file and link the URL, in quotation marks, in the audiovideo-id. You can store mp3s in your GitHub repository, but be aware that GitHub only allows a small amount of space to each repository. It's probably best practice to link them from elsewhere. You will also need to change av_source to "mp3". Follow the visualizations below for instruction. 

- If you have a page for your mp3 file copy the URL. 

{% include bootstrap/figure.md img="howto/url_mp3_final.png" caption="" alt="mp3 page URL" %}

- Copy and paste URL with quotation marks included. 

{% include bootstrap/figure.md img="howto/final_source.png" caption="" alt="Included URL for mp3 feature" %}

- Change *av_source* to "mp3". 

{% include bootstrap/figure.md img="howto/url_mp3_final.png" caption="s" alt="av_source edited to include mp3 file" %}



## Step 5: Setting up the visualization(s)

{:.alert .alert-info}
OHD offers a way to categorize your transcripts using tags. This is done through two locations: the "tag" column cells in your transcript's CSV and the filters.csv file, which is already provided for you in the structure of OHD. If you are not aware of either of these files, first visit our steps on "[How To Prepare Your Data](prepareyourdata.html)." 


{% include youtube/embed.html  video-id="esUuJbhXKW4" title="Creating Filters" display="d-none d-md-block" %}
- Open the filters.csv file you created in your text editor. 
- Navigate to the "_data" folder 
- Open the "_data" folder and click the pencil icon to edit the file
- Copy and paste the filters.csv you created in the Prepare Your Data tutorial over into the existing content. 
- Alternatively, you can simply edit the CSV file here. (Below is how the file looks when opened with the pencil icon.)
{% include bootstrap/figure.md img="howto/texteditorfile.png" caption="Filters.csv as it looks in a text editor" alt="opened file, ready for editing" class="w-50" %}
{% include bootstrap/figure.md img="howto/githubfile.png" caption="filters.csv copied into GitHub" alt="filters.csv copied into GitHub" class="w-50" %}
- Commit the change at the bottom of the page by clicking the commit button (be sure to write a commit message so you can track your changes)
{% include bootstrap/figure.md img="howto/commit_file.png" caption="" alt="picture of the commit button at bottom of page" class="w-50" %}
- However you edited it, the finished CSV should look like the example below (with your new tags and descriptions) in GitHub
{% include bootstrap/figure.md img="howto/githubfilefinal.png" caption="CSV after being transferred to GitHub" alt="finished csv after being transferred to github" class="w-50" %}
- Below is a slightly more robust example of what your visualization will look like. 
{% include bootstrap/figure.md img="howto/visualization.png" caption="finished OHD visual" alt="picture of finished visualization" class="w-50" %}




