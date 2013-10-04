---
title: Lesson 3
author: Dan Hahn
date: 2013-10-02
template: article.jade
---

#Including a CSS File

* [Intro to CSS]()
* [Selectors](selectors.html)
* [Include File](include.html)
* [CSS2 Properties](css.html)
* [Homework](homework.html)

To include a css file in an HTML the first thing you need is a .css file.  You can create a .css file the same way you create a .html.  Go to file save as and give the file a name and add .css as the extension.

##Link Tag

The link tag is an HTML tag that is added within the head of a document.  This tag has three attributes.

* `href` – the location of the file
* `rel` – set to stylesheet
* `type` – set to text/css - *Not needed with HTML5*

###Example

	<link rel=”stylesheet” type=”text/css” href=”filelocaiton.css”/>

---

##@IMPORT

`@import` includes a `.css` but does it with in CSS itself.  With `@import` one css file can include another file.

###Example

	<style type=”text/css”>
		@import url(filename.css);
	</style>

---

##Print CSS
CSS files can be targeted to only the screen or printer.  This allows different styles to be applied to the screen and the printer.

###Example

For full file

	<style type=”text/css”>
		@import url(filename.css) print;
	</style>

Within a style block

	<style type=”text/css”>
	h2 {
		color: blue;
	}
	@media print {
		h1 {
			color: black;
		}
	}
	</style>

##Using Link

	<link rel=”stylesheet” type=”text/css” href=”filelocaiton.css” media=”print”/>

---

##MEDIA TYPES

* `all` – Suitable for all devices.
* `handheld` – Intended for handheld devices (typically small screen, limited bandwidth).
* `print` – Intended for paged material and for documents viewed on screen in print preview mode. Please consult the section on paged media for information about formatting issues that are specific to paged media.
* `screen` – Intended primarily for color computer screens.

