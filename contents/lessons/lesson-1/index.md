---
title: Lesson 1
author: the-wintersmith
date: 2013-09-18
template: article.jade
---

Introduction to HTML, Web Browsers, Standards

<span class="more"></span>

#Introduction

* [Intro]()
* [Blocklevel](blocklevel.html)
* [Homework](homework.html)

[Download Notes <i class="icon-download-alt icon-white"></i>](week1-notes.zip)


##HTML stands for HyperText Markup Language.

1. **Hypertext** is ordinary text that has been dressed up with extra features, such as formatting, images, multimedia, and links to other resources.
2. **Markup** is the process of taking ordinary text and adding extra symbols. Each of the symbols used for markup in HTML is a command that tells a browser how to display the text.

##Make up of HTML Element (Tag)

Element – the type of HTML tag.

	<h1>ephemeral</h1>

Each Element will have at least 3 parts

1. `<` - opening bracket
2. tag name – how the browsers should hand this tag
3. `>` - closing bracket

Most tags will have an additional closing tag that is just like opening tag but with an indication that it is an ending tag. `</h1>`. In case where the element does not have a closing element you must add a / at the end of the tag.

	<br /> or <hr />

##Attributes and values

Attributes contain in formation about the data in the document as opposed to being that data. Attributes values must always be contained in double quotes (“). Each HTML element has its own set of attributes and values. Attributes applied to elements that do not support them will disregard at the time of rendering.

	<img src=”bluecat.jsp” />

Many Elements allow for multiple attribute.

	<img src=”bluecat.jsp” width=”300” />

Attributes will only be added to the opening element

	<td colspan=”3”>Month</td>

##Block vs Inline

HTML elements are divided in to two types Block-level elements or inline elements.

* Block-level elements are more structure elements. Block-level elements will always start a new line.
* Inline elements used for formatting elements. If you want a word to be bold with in a paragraph.

##Ordering of tags
Block level elements should always be the outer most tags. Tags should be closed in the opposite order they where opened. (First in / Last out).

	<div><b><i>example</i> text </b></div>

Notice how the elements are open and closed.

##File Names

All file names should be lower case and never have spaces or any special characters and will always end with the extension .html

	capital_punishment.html

##Saving a file.

When you create a HTML file you will need to save it with an .html extension. This will tell the browser to that the file is HTML and should display the HTML in the page. The text editor will not know to add an .html extension so you will have to add it by hand.

1. Don’t just click save you must use Save As
2. Navigate to the location that you want to save your file.
3. Give your file a name. It should never have any spaces or special character in it. Instead of a space you can user an underscore “_”
4. After the name you will need to type “.html” This will make the file an HTML file.
5. Click Save.

##Viewing an HTML file in a web browser.

Now that you have created an HTML file you will need to view your file in a web browser. This will remove the HTML that you have written and render it the way that you want it to look. Since we are working locally (all files saved on our hard drive) we well have to navigate to the file and open it.

1. Click on file.
2. Select open file.
3. Navigate to the file that you want to open.
4. Click open.

##Editing a file that you have already created

You can not just double click on a file that you have saved as an HTML file. If you do that it will open in the web browser. To edit in the text editor you will need to open it directly.

1. Click file
2. Select open.
3. Navigate to your file.
4. Click Open.

##Alternative Text Editors

There are a number of text editors that you can use to write your code outside of class. 

* TextEdit – Installed on all macs.
* TextWrangler – Macs Only (free) - http://www.barebones.com/products/textwrangler/download.html
* Sublime Text 2 – Mac and PC (free) - http://www.sublimetext.com/2
* TextMate – Mac only (fee) - http://macromates.com/
* Coda 2 – Mac only (fee) - http://panic.com/coda/
* NotePad++ – PC only (free) - http://notepad-plus-plus.org/
