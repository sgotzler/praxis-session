# Building a Jekyll site

## What is Jekyll?

Jekyll is a simple, static website generator. It utilizes what's called "markup," rather than a back-end database, to create its webpages. As such, Jekyll websites can be securely deployed on the web with minimal maintenance in an easily preservable format, usually for free. 

Such a format allows us to freely host a website, for example, and to collaborate across a research team, and integrate the principles of minimal computing we seek to use when creating digital reading editions for the public or the classroom. 

Jekyll utilizes what's called the Ruby programming language. Ruby uses "gems" to install the necessary packages required to run certain programs. Jekyll is thus one "gem" running within Ruby, and you will need to install both Ruby and the Jekyll gem on your computer before you can run a Jekyll site. 

How to do this is outlined for both MacOS and Windows in the [following helpful guide](https://programminghistorian.org/en/lessons/building-static-sites-with-jekyll-github-pages#text-editor-).

## Integrating "Ed." with your Jekyll site

“Ed.” is a Jekyll theme. It sits on top of a basic Jekyll site, within Ruby. "Ed." is a customized version of the basic Jekyll site built by Alex Gil and others, which greatly enhances both the style and functionality of a Jekyll website. 

Once a basic Jekyll website has been created, swapping out the default Jekyll theme for “Ed." is pretty easy to do. To do so, you’ll need to edit two things: (1) the "config.yml" file and the gem file using what's called a text editor. How to do this is outlined in [Ed’s documentation](https://elotroalex.github.io/ed/documentation/#installing-ed-replacing-an-existing-jekyll-theme).

## GitHub and working with the Command Line

To start with, then, a Jekyll site requires three things: (1) access to Github, (2) access to the command line of your computer to install the "gem" etc., and a text editor.

* **GitHub** is a code hosting platform for keeping track of versions of a computing project and for collaboration. Github lets you build, store, manage and collaborate on digital projects with others from anywhere with internet access.

    - For more information about getting started using GitHub see their [Hello World Guide](https://guides.github.com/activities/hello-world/#what).
    
* **Command Line** -- To launch a Jekyll site you'll first need to familiarize yourself with some very basic aspects of "a command line interface (or CLI)," sometimes called "Bash Command Line." A Command-Line Interface, as opposed to the Graphical User Interface (or GUI) that most of us are familiar with, differs in that it allows users to issue text-based commands to their computer through a terminal window or "shell." 

>**NOTE**: Working in GitHub and installing some of the necessary components for running Jekyll requires a brief amount of work, up-front, in the command line--however once this work has been done, all maintenance can be done with the [GitHub Desktop Client](https://desktop.github.com/), an easy to understand GUI that works like any other app. 

Put another way, a minimal amount of computing upfront will reap you large rewards, as you'll be able to build sites from now on with GitHub Pages, using a GUI, without using the command line at all.
 
* **Text Editors** -- Lastly, in order to work with Jekyll to build a static website you'll need to use a text editor to view, edit, and save changes to the pages that compose your website's content and structure. 

    - We will touch on text-editors in our next section on "Markdown," but if you're interested in learning more about how to build your own Jekyll site you should refer to [this reading](https://programminghistorian.org/en/lessons/building-static-sites-with-jekyll-github-pages#text-editor-) from Amanda Visconti's "Building a static website with Jekyll and GitHub Pages," full version linked below.

### Further Resources

* [Link to Introduction to the Bash Command Line](https://programminghistorian.org/en/lessons/intro-to-bash)
* [Building a static website with Jekyll and GitHub Pages](https://programminghistorian.org/en/lessons/building-static-sites-with-jekyll-github-pages)
* [Documentation for *Ed.*, a theme for minimal digital editions](https://elotroalex.github.io/ed/documentation/#installing-ed-replacing-an-existing-jekyll-theme)
* [Quick Start Guide for Jekyll builder](https://jekyllrb.com/docs/)
* [GitHub Pages Tutorial](https://pages.github.com/)
