# Editing and Writing with Markdown

Developed in 2004 by John Gruber, "Markdown" is the name of a lightweight markup language you can use to add formatting elements to plain text files. 

A markup language is a way of formatting and enriching plain text (e.g. adding headers, tags, hyperlinks, etc.) Also, Markdown is increasingly the most commonly used form of markup language for DIY web-development projects. 
 
**Markdown has many advantages over HTML:**

* Minimizes reliance on proprietary platforms by offering a stripped down, easy-to-use markup language that allows people to render texts quickly and efficently on their own static websites, (i.e.avoiding services like squarespace or word press).

* Reduces reliance on specialized techinal language making digital projects both: 
   - transparent (readability)
   - reproducible (accessiblity)

The main drawback is that design choices for styling plain text are limited using Markdown. For instance, some working knowledge of CSS and Java is still necessary to tweak and customize most Jekyll websites, if you want them to look like corporate websites.

## Importing Your Own Text 

Once you've decided on a text you'd like to use to create a digital reading edition, you might need to convert it to plain text before "marking it down" to prepare it to be rendered for the web. One common example is when you have a pdf of a text that you would like to add to your website in plain text. 

### Converting pdf's to plain text using Calibre

*Calibre* is a handy e-book mgmt. software with many interesting features that is available for free. Among other things, it allows you to easily convert pdf's to plain-text. 
* You can download Calibre [here](https://calibre-ebook.com/).

>**NOTE**: The ease of converting pdfs to plain text depends on the condition of your primary text (hand-written or scanned pages will present further difficulties and require preliminary optical character recognition (OCR) to work. *Calibre* will only work smoothly with pdf's that do not need to be OCR'ed.

* **DEMO: Converting PDF to plain-text with *Calibre* (Raymond Williams, "The Future of Marxism")**

### Creating HTML files from websites

Another option might be to locate an online version of a text presented on the web in HTML and to download it using an automated program.

In fact, this is what we did for *MARXdown* using an existing HTML text on [marxists.org](https://www.marxists.org/archive/marx/works/1867-c1/) for *Capital Vol.1*. 

To execute this task we used a command line program called *Wget*. *Wget* retrieves content from the web and saves that data locally on your machine as per the existing site structure (for example, in nested folders with .HTML files).

For *MARXdown* we used the following code:

```bash
wget -r --no-parent -w 2 --limit-rate=20k https://www.marxists.org/archive/marx/works/1867-c1/
```
>**NOTE**: When using *Wget* you need to be aware of the website's structure such as security (SSL Certificates), or dynamically created sites (javascript versus python, etc.)--marxists.org is created using farily basic HTML, so it was easy to retrieve. More complex sites will require more programatically sophisticated methods. 

>Also, please be aware of how much data you are downloading at once, and be careful not to overload the website's servers. It is generally good practice to put in a wait time of 1-2 seconds--you can see we did this by adding "-w 2" in the line of code above.

Executing an automated download of marxists.org required a bit more in-depth editing work on our part, after we had aquired the HTML. We had to remove all of the HTML tags and formatting, for example, replacing hyperlinks, and essentially translating from HTML to Markdown. 

But it also promised us the ease of plain text acquisition; in otherwords, we quickly acquired an open copyright plain text copy of the book in its entirety without having to deal with OCR or file conversion processes.

## Working with Text-Editors: *Atom*, *Sublime*

Once you've OCR'ed your scans of documents, converted your PDF, or retrieved your website for the underlying HTML files, you'll need to work in a text-editor to begin re/writing and editing the text in Markdown.

* There are numerous options for text editors, some of the most popular include [Sublime](https://www.sublimetext.com/) and [Atom](https://atom.io/), but you can also find several online "live" markdown editors, where you can copy/paste a plain text file, and begin to see your changes rendered as you make them.

>**NOTE**: Grab the plain text copy of the Raymond Williams which I've dropped in the [repo](https://github.com/sgotzler/praxis-session/blob/master/The%20Future%20of%20Marxism%20-%20Raymond%20Williams.txt). 
If you already have a text-editor feel free to work in that. Otherwise, copy and paste it into this in-browser markdown editor: [StackEdit](https://stackedit.io/)

* **DEMO: "marking-down" a plain text file**
  - Check out a finished version [here](/praxis-session/williams-final).

### Further Resources
* [Tips on How to Convert PDF to ePUB with *Calibre* and its Settings](https://pdf.iskysoft.com/convert-pdf/convert-pdf-to-epub-with-calibre.html)
* [Automated Downloading with *Wget*](https://programminghistorian.org/en/lessons/automated-downloading-with-wget)
* [Markdown Guide and Cheat Sheet from markdownguide.org](https://www.markdownguide.org/cheat-sheet/)
* [Sustainable Authorship in Plain Text using Pandoc and Markdown by Dennis Tenen and Grant Wythoff](https://programminghistorian.org/en/lessons/sustainable-authorship-in-plain-text-using-pandoc-and-markdown)


### [Next Section](/praxis-session/hypothesis)
