# Building a Jekyll site

## What is Jekyll?

Jekyll is a simple, static site generator. It utilizes markup, rather than a back-end database, to create webpages. As such, these sites can be securely deployed on the web with minimal maintenance in an easily preservable format. 

This format allows us to freely host a website, collaborate across a research team, and integrate the principles of minimal computing we sought to use when creating our digital reading edition. 

Jekyll utilizes the Ruby programming language. Ruby utilizes ‘gems' to install the necessary packages required to run programs. Jekyll thus is a ‘gem’ within Ruby, and you need to install the Jekyll gem in before running the program. 

All of these dependencies and their installations are outline for both MacOS and Windows in the [following guide](https://programminghistorian.org/en/lessons/building-static-sites-with-jekyll-github-pages#text-editor-).

## Integrating "Ed." with your Jekyll site

“Ed.” is a theme which sits on top of a basic Jekyll site. It is a customized version of the basic site that enhances both the style and functionality. 

Once a basic Jekyll site has been created, swapping out the basic Jekyll theme for “Ed." is easy. To do so, you’ll need to edit both the config.yml and gem file with a text editor. This is explained in more detail in [Ed’s documentation](https://elotroalex.github.io/ed/documentation/#installing-ed-replacing-an-existing-jekyll-theme)

## GitHub and working with the Command Line

A Jekyll site requires Github, access to the command line, and a text editor.

* **GitHub** is a code hosting platform for version control and collaboration. It lets you build, store, manage and collaborate on digital projects with others from anywhere with internet acces.
    - For more information about getting started using GitHub see their [Hello World Guide](https://guides.github.com/activities/hello-world/#what).
    
* **Command Line** -- To launch a Jekyll site you'll need to familiarize yourself with working in a command line interface. A Command-Line Interface, as opposed to a Graphical User Interface (or GUI), allows users to issue text-based commands to their computer through a terminal or "shell." 

>**NOTE**: Working in GitHub and installing some of the necessary components for running Jekyll requires a brief amount of work, up-front, in the command line -- however once this has been done, all maintenance can be done with the [GitHub Desktop Client](https://desktop.github.com/) GUI, and building a site with GitHub Pages without using a CLI at all, see link below.
 
* **Text Editors** -- In order to work with Jekyll to build a static website you'll need to use a text editor to view, edit, and save changes to the pages that compose your site's structure. 
    - We will touch on text-editors more in the next section, but if you're interested in building your own jekyll site you might refer to [this section](https://programminghistorian.org/en/lessons/building-static-sites-with-jekyll-github-pages#text-editor-) from Amanda Visconti's "Building a static website with Jekyll and GitHub Pages," full version linked below.

### Further Resources

* [Link to Introduction to the Bash Command Line](https://programminghistorian.org/en/lessons/intro-to-bash)
* [Building a static website with Jekyll and GitHub Pages](https://programminghistorian.org/en/lessons/building-static-sites-with-jekyll-github-pages)
* [Documentation for *Ed.*, a theme for minimal digital editions](https://elotroalex.github.io/ed/documentation/#installing-ed-replacing-an-existing-jekyll-theme)
* [Quick Start Guide for Jekyll builder](https://jekyllrb.com/docs/)
* [GitHub Pages Tutorial](https://pages.github.com/)
