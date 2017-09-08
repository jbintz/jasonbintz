---
title: 'Science Honors: Assignment 4'
author: ''
date: '2017-09-08'
slug: science-honors-assignment-4
categories: []
tags: []
---

The topics for the next three Tuesday class meetings are:

-  measuring biodiversity
-  estimating biodiversity
-  comparing biodiversity

I have developed a set of tutorials to guide you into these rich topics. The format of the tutorials--*not* the content--is similar to the one I called the "setup tutorial."

Here's another example of this kind of tutorial. **Do not complete this tutorial!** I only want you to get a sense of its format. Here's the link: <https://jjallaire.shinyapps.io/learnr-tutorial-01-data-basics/>

Navigate to the Data Frames tab. Notice that there is some information about data frames followed by a question and an R chunk for you to use to answer the question. You can enter R code, run it and submit your answer. 

How did the author create this tutorial? Under the hood, this is simply an R Markdown document! It has a special output format that, when the .Rmd file is "run", the result is the tutorial. Of course, you don't see the raw .Rmd file; you see the output of it. The author has published this tutorial and it is hosted on the web via shinyapps.io by RStudio. 

I could, in theory, do the same thing. There are two reasons I'm electing not to do that. One reason is that I'd have to pay to use that service! The other reason is that it isn't necessary. You can run the exact same tutorial on your local machine if you have the raw .Rmd file. You simply open the file in RStudio and "run" it. The purpose of this assignment is to ensure that you can successfully do this on your laptop.

1.  Open RStudio. I recommend you open RStudio by opening the project we created at the woRkshop.

1.  Install the `learnr` package by running the command `install.packages("learnr")`. Go ahead and also install the `nycflights13` package.

1.  Close and reopen RStudio.

1.  *File -> New File -> RMarkdown...*

1.  In the popup window, choose "From Template". You should see an option called "Interactive Tutorial". Highlight this option and name the document `data-basics` and click OK.

1.  Two things should have happened. First, a folder named `data-basics` was created in your current working directory, and, second, the file `data-basics.Rmd` was created. This file lives inside the folder `data-basics` and you should see it open in the source panel inside RStudio. It begins with a yaml header that looks like this:
    ````
    ---
    title: "Tutorial"
    output: learnr::tutorial
    runtime: shiny_prerendered
    ---
    ````
    
1.  Just like a notebook or rmarkdown document, this tutorial template is pre-populated with some basic ingredients. Go ahead and click the "Run Document" button and check out the output that is created. Compare and contrast the output with the raw file.

1.  I want you to now erase the contents of the file. **I do not want you to delete the file**, I only want you to erase the contents, ok?

1.  We are now going to paste into this (now blank) document the raw .Rmd file that created the data basics tutorial that you just visited. You want to verify that you can reproduce the same thing on your local computer.

    a.  Navigate to this [link](https://raw.githubusercontent.com/rstudio/learnr/master/examples/01-data-basics/01-data-basics.Rmd), highlight the entire page and copy to your clipboard.
    
    b.  Back to RStudio, place your cursor at the top of your blank document and paste the content of your clipboard into the document.
    
    c.  Finally, run the document and verify that you have reproduced the tutorial you visited earlier on the Web.