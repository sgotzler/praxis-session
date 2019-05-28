# Editing + Writing with Markdown

What is markdown?

Developed in 2004 by John Gruber, Markdown is a lightweight markup language that you can use to add formatting elements to plaintext files. A markup language is a way of formatting and enriching text (e.g. adding headers, tags, hyperlinks, etc.) 

Markdown is increasingly the most commonly used form of markup language for DIY web-development projects. 
 
Advantages over html: 
* Minimizes reliance on proprietary platforms by offering a stripped down, easy-to-use markup language that allows people to render texts quickly and efficently on their own static websites, (i.e.avoiding services like squarespace or word press).

* Cuts down reliance on specialized techinal language making digital projects both: 
   - a) transparent (readability)
   - b) reproducible (accesiblity)

The major drawback is that design choices are limited. 

For instance, some working knowledge of CSS and Java is still necessary to tweak and customize most jekyll sites. A site written in markdown only will be static, and more than likely soley text/hypertext based.  

## Importing Your Own Text 

Once you've acquired a text you'd like to use to create a digital edition, you'll need to convert it to plain text before using "marking it down" to prepare it to be rendered for the web.

### Converting pdf's to plain text using Calibre

*Calibre* is an e-book mgmt. software that is available for free, and allows you to easily convert pdf's to plain-text. 
* You can download it [here](https://calibre-ebook.com/).

>**NOTE**: The ease of this process depends on the condition of your primary text (hand-written or scanned pages will present further difficulties and require preliminary optical character recognition (OCR) work. *Calibre* will only work smoothly with pdf's that do not need to be OCR'ed.

* **DEMO: Converting PDF to plain-text w/ *Calibre* (Raymond Williams, "The Future of Marxism")**

### Scraping websites to create html files

Another option might be to locate a public domain online version of a text and download an existing website to receive the source information as a ".html" file using an automated program.

This is what we did for *MARXdown* using the existing text on [marxists.org](https://www.marxists.org/archive/marx/works/1867-c1/) for *Capital Vol.1*. 

To execute this task we used a command line program called *Wget*. *Wget* retrieves content from the web and saves that data locally on your machine as per the existing site structure (i.e. nested folders and .html files).

For *MARXdown* we used the following code:

```bash
wget -r --no-parent -w 2 --limit-rate=20k https://www.marxists.org/archive/marx/works/1867-c1/
```
>**NOTE**: When using *Wget* you need to be aware of the website structure such as security (SSL Certificates), dynamically created sites (javascript, python, etc.) -- marxists.org is created using farily basic html, so it was easy to scrape. More complex sites will require more programatically sophisticated methods. 
>Also, be aware of how data you are downloading at once and be careful not to overload the website's servers. It is generally good practice to put in a wait time of 1-2 seconds "-w 2" in the line of code above.

Executing an automated download of marxists.org required a bit more in-depth editing work on our part, removing all of the html tags and formatting, replacing hyperlinks, and essentially translating from html to markdown. 

But it also promised the ease of plaintext acquisition, i.e. we quickly acquired an open copyright plain text copy of the text in its entirety with out having to deal with OCR or file conversion processes.

## Working with Text-Editors: *Atom*, *Sublime*, etc.

Once you've OCR'ed your scans of documents, converted your PDF, or scraped your website for the underlying html files, you'll need to work in a text-editor to begin re/writing and editing the text in markdown.

* There are numerous options for this, some of the most popular include [Sublime](https://www.sublimetext.com/) and [Atom](https://atom.io/), but you can also find several online "live" markdown editors, where you can copy/paste a plain text file, and begin to see your changes rendered as you make them.

>**NOTE**: Grab the plain text copy of the Raymond Williams which I've dropped in the [repo](https://github.com/sgotzler/praxis-session/blob/master/The%20Future%20of%20Marxism%20-%20Raymond%20Williams.txt). 
If you already have a text-editor feel free to work in that. Otherwise, copy and paste it into this in-browser markdown editor: [StackEdit](https://stackedit.io/)

* **DEMO: "marking-down" a plain text file**
  - Check out a finished version [here](/praxis-session/williams-final).

### Further Resources
* [Tips on How to Convert PDF to ePUB with *Calibre* and its Settings](https://pdf.iskysoft.com/convert-pdf/convert-pdf-to-epub-with-calibre.html)
* [Automated Downloading with Wget](https://programminghistorian.org/en/lessons/automated-downloading-with-wget)
* [Markdown Guide and Cheat Sheet from markdownguide.org](https://www.markdownguide.org/cheat-sheet/)
* [Sustainable Authorship in Plain Text using Pandoc and Markdown by Dennis Tenen and Grant Wythoff](https://programminghistorian.org/en/lessons/sustainable-authorship-in-plain-text-using-pandoc-and-markdown)
