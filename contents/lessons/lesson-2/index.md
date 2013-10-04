---
title: Lesson 2
author: Dan Hahn
date: 2013-09-25
template: article.jade
---

This week we will talk about how to create links and embed images.

<span class="more"></span>

# Anchor Tag (inline element)

* [Link Tag]()
* [Folder](folders.html)
* [Images](images.html)
* [Image Types](image-types.html)
* [Image Examples](image-examples.html)
* [Homework](homework.html)

[Download Notes <i class="icon-download-alt icon-white"></i>](lesson2-notes.zip)[Download Stater File <i class="icon-download-alt icon-white"></i>](lesson2.zip)


The anchor tag or the `<a>` tag is most commonly used to create a link to an other file or page.  The anchor tag by default will not act as a link without the `href` attribute.  

The anchor tag can also be used to set a point on a page where the page can be linked to.  You might see this on an FAQ page where you have a list of questions at the top and the answers at the bottom. 

Please note there is not a link tag.  If someone askes you to create a link they are talking about the anchor tag. 

##Example
`<a href=”http://www.sva.edu”>http://www.sva.edu</a>`

**or**

`<a name="pointname">Page Content</a>`


###Description


Attributes|Value|Description
---|---|---
`href=””`|URL|The target URL of the link
`target`|`_blank`|Where to open the target URL. `_blank` - the target URL will open in a new window

---

## Parts of a link

There are two parts to create a link

1. The text or content the user can click on
2. The location of the page the user will have the page replace.

### Example

`<a href="location/of/file.html">Clickable text</a>`

#### Breaking it down

Lets start with the `<a>` which is added to create the anchor.  Next we need to add the `href` **attribute** to make the anchor act as a *link*. Then we wrap the text we want the user to click on with the `<a>`. Last we add the location of the page we want to link to. 

If we had the text **HTML at SVA** and wanted to link to the web page *http://www.svahtml.com* the link would look like this.

`<a href="http://www.svahtml.com">HTML at SVA</a>`

Keep in mind that the `<a>` is an inline element so it can be placed next to other text. 

If you want a link to be on its own line it would need to wrapped with a blocklevel element like a `<p>`.

---

##Linking to a file in the same folder

When you link to a file that is in the same folder just add the file name to the HREF attribute.

`<a href="filename.html">Link Text</a>`

##Linking to a file in a sub folder

When linking to a file in a sub folder you need to declare what folder you are navigating to then add the file.

`<a href="folder/filename.html">Link Text</a>`

##Linking to a file in a parent folder

When linking a file in a parent folder you need to add `"../"` for each folder you want to navigate up.  You do not need the folder name when navigating up.

`<a href="../filename.html">Link Text</a>`

##Linking to an outside site

When linking to an outside site you need to add the full URL including the `http://`.

`<a href="http://www.svahtml.com">Link Text</a>`

##Linking to a point with a page.

The link add the "#" that says look on the page for a A tag with a name that matches the text after the #.

`<a href="#sectionName">Link to section</a>`

The point on the page you are linking to.

`<a name="sectionName"></a>`

##Images as a link

###Example
`<a href=”http://www.cnn.com”><img src=”/images/cnnlogo.png” alt=”link to cnn” border=”0”/></a>`



<style>
table tr td:nth-child(1){width:20%}
</style>