I had an issue where one of my timestamps was only in minutes and seconds and the templating language here, Liquid, only read it as Hours and Minutes, thus messing up the math that makes the links work. I edited it by using this regular expression based find an replace: 

Find: `\[([0-9][0-9]:[0-9][0-9])\]`
Replace: [00:$1]

