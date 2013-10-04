---
title: Lesson 1
author: the-wintersmith
date: 2013-09-18
template: article.jade
---

#Basic HTML Structure

* [Intro]()
* [Blocklevel](blocklevel.html)
* [Text Edit](textedit.html)
* [Homework](homework.html)

##Creating an HTML page (basic template)

Because over the year there have been many version of HTML we need to define on each HTML document what version of HTML is used on the page. This is done with the DOCTYPE. Doctype is not really an HTML element but a definition of HTML. Unless you are a very advanced user you will use the same doctype over and over.

We will use this DOCTYPE for all our pages.

`<!DOCTYPE html>`

This is an HTML5 doctype

##`<html>` Element
`<html>` - Tell the browser that the document is an HTML file and should render it such. The `<html></html>` Element should be the first element after the DOCTYPE and the last element within the HTML document.

##`<head>` Element

The head element can contain information about the document. The browser does not display the "head information" to the user. The following tags can be in the head section: `<base>`, `<link>`, `<meta>`, `<script>`, `<style>`, and `<title>`

##`<body>` Element
The body element defines the documents' body. It contains all the contents of the document (like text, images, colors, graphics, etc.).

##Adding a page title
Each HTML Document need to have a page title. The page title will not display on the screen but will appear in the browser's title bar. A title is required for each document.

To add at title to the document you will nest the `<title></title>` within the <head> element.
###Example

	<head>
		<title>Page Title</title>
	</head>

You can name your title anything you want. I should be name something relating to the page contents. This is also the best way to get what the page contents are about to search engines like google.

###Template Example

	<!DOCTYPE html>
	<html>
	<head>
		<title></title>
	</head>

	<body>

	<body>
	</html>

All other HTML elements that the one listed in the `<head>` Tag will be nested with the body Element.

##Structure Tags - Block Level Elements

###Section Headers (h1 to h6)

HTML provides for up to six levels of headers for your web page. `<h1>`, `<h2>`. `<h3>`, `<h4>`, `<h5>`, `<h6>`. Headers sometime called headlines are block-level elements there for they will always create new line. In addition they will make the text bold and change the size of it depending on the number next to the `<h1>` is the largest and `<h6>` is the smallest.

Section headers should be used to define the important of the content. So there should only be one H1 on a page but there could be many H2s on a page since they would be viewed as sub header of the H1 and so on.

###EXAMPLE

	<h1>Article Title</h1>
	<h2>Article Subsection</h2>
	<h3>SubHeader</h3>
	<h2>Article Subsection</h2>

###Paragraph Element (<p>)

Since HTML will not display line breaks within the HTML source to get that formatting to display within the browser we need to use the paragraph tag.
`<p></p>`. The paragraph tag is a block-level element. It will add a small amount of space above and below the element.

####EXAMPLE

	<p>sample text</p>

Breaking up a Page into Divisions (<div>)

Breaking the page up into divisions allows you to apply styles to an entire chunk of your page at once. This can also be used to layout your page. The <div> element is a block-level element but has not margin applied like the paragraph tag.

With the div element you will apply an attribute of class or id to apply a style to it.

####EXAMPLE

	<div>
		<h2>Article Subsection</h2>
		<p>sample text</p>
		<p>sample text</p>
		<p>sample text</p>
	</div>

###Creating line break
The `<br>` tag inserts a single line break.

The `<br>` tag is an empty tag.

####EXAMPLE

	<p>This example is<br> <span>very important</span></p>

###List - `<ul>`, `<ol>`, `<li>`
List are built into HTML and come in two types, ordered and unordered. List are made up of at least two tags the `<ul>` or `<ol>` and the `<li>`.

The `<ul>` or `<ol>` will add a margin at the top and the bottom of the list along with indenting the list on the left side.

Tag|Description
--|--
`<ul></ul>`|Unordered list – bullets
`<ol></ol>`|Ordered list – numbers
`<li></li>`|List Item.

###example
##Unordered list

	<ul>
		<li>List item</li>
		<li>List item</li>
		<li>List item</li>
	</ul>

Ordered List

	<ol>
		<li>List item</li>
		<li>List item</li>
		<li>List item</li>
	</ol>

###Example

	<div>
		<h1> Lorem ipsum dolor sit amet </h1>
		<p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Maecenas quis augue ut massa nonummy viverra. <a href=”http://www.lorenipsum.com”>Cras convallis pulvinar</a> ante. Proin varius velit eget tellus. Duis elit. Quisque lectus velit, consequat sed, nonummy quis, molestie vitae, nisl. Praesent vehicula, odio vitae </p>
		<ul>
			<li>List Item</li>
			<li>List Item</li>
			<li>List Item</li>
		<ul>
	</div>

###Nested List Item

You can nest a list with in a list but it must be added to a list item

	<ul>
		<li>
			Item Text
			<ul>
				<li>Sub List Item</li>
			</ul>
		</li>
	<ul>

##Blockquote

A browser inserts white space before and after a blockquote element. It also insert margins for the blockquote element.

	<blockquote>
		<p>Here is a long quotation here is a long quotation</p>
	</blockquote>

##New HTML5 Tags

TAG|DESCRIPTION
--|--
`<article>`|Defines an article
`<aside>`|Defines content aside from the page content
`<details>`|Defines additional details that the user can view or hide
`<figure>`|Specifies self-contained content, like illustrations, diagrams, photos, code listings, etc.
`<footer>` |Defines a footer for a document or section
`<header>`|Defines a header for a document or section
`<nav>`|Defines navigation links
`<section>`|Defines a section in a document

