# HTML_Syntax
[Developement Notebook](Table%20of%20Contents.md)
_______________________________________________________

## Table of Contents
**[HTML_Concepts](#HTML_Concepts)**

**HTML_Elements**

[Header](#Header) <br>
[Paragraph](#Paragraph) <br>
[Boldface](#Boldface) <br>
[Italic](#Italic) <br>
[Newline](#Newline) <br>
[Anchor](#Anchor_(aka_Link)) <br>
[Image](#Image) <br>
[List](#List) <br>
[Head](#Head) <br>
[Title](#Title) <br>
[Body](#Body) <br>
[HTML](#HTML)


**Questions**

[Open_Questions](#Open_Questions)

**[References](#References)**
_______________________________________________________

## HTML_Concepts

HTML is a languge composed of discrete "elements". Elements are composed of three syntactic parts, the opening tag, the content, and the closing tag. In the most basic sense, html puts content into buckets. The content is provided by the user and the name of the bucket is specified using html. That is all it does. HTML does not determine how things look on the page. The way that happens is that CSS assigns styling factors to buckets. Using these two languages, content and styling factors end up in a bucket and the browser collects and organizes all the buckets into a nested scheme and then renders it. By default some html elements already have default css styling. These are elements that represent intuitive aspects of writing and print like paragraphs, boldface, and headers. There are other html elements that correspond to regular writing and visual layout concepts like a header, footer, side panel, etc. These preset html elements are called "semantic". You will probably use a handful of them; But if you are going to get into more advanced web design then it will not take you too long to move beyond them.

HTML Element: Header 1 Element
```html
<h3> This is a header </h3>
```
<h3> This is a header </h3>

The `<h3>` is the opening tag and specifies the bucket will be `Header #3` element. The content, what will actually be written in the header style, is `This is a header`. And the closing tag is `</h3>`. All closing tags will start with the forward slash, `/`. All tags are composed of a name sequence, `h3`, inside a set of angle brackets, `<>`. Many tags will also include specifiers within the opening tag. Ex `<h1 class="class 1"> Class 1 </h1>`. More on that later.       

_______________________________________________________
## HTML_Elements

### Header
```html
<h1> Header 1 </h1>
<h2> Header 2 </h2>
<h3> Header 3 </h3>
<h4> Header 4 </h4>
<h5> Header 5 </h5>
<h6> Header 6 </h6>

```
<h1> Header 1 </h1>
<h2> Header 2 </h2>
<h3> Header 3 </h3>
<h4> Header 4 </h4>
<h5> Header 5 </h5>
<h6> Header 6 </h6>

_______________________________________________________
### Paragraph
```html
<p> Paragraphs just look like normal test </p>
```
<p> Paragraphs just look like normal test </p>

_______________________________________________________

## Boldface
The tag name for bondface elements is `strong`. It seems a strange and unintuitive thing to use, but that is just how it is unfortunately.

```html
<strong> This is how to bold something in html </strong>
```
<strong> This is how to bold something in html </strong>

_______________________________________________________

## Italic
Same deal as boldface, `em` is a strange and unintuitive name to me, but that is just the way it is, sadly.

```html
<em> This is how to italicize something in html </em>
```
<em> This is how to italicize something in html </em>

_______________________________________________________

## Newline
Unlike other elements so far, this one has no content and therefore only requires an opening tag.
```html
This will be a line above<br>and this will be a line below
```
This will be a line above<br> and this will be a line below

_______________________________________________________
## Anchor_(aka_*Link*)
The anchor tag is one of the first tags with content inside the opening tag. HTML elements have 'attributes' that can be specified inside of the tags. The href attribute is one associated with the anchor element. The anchor element is used to create hyperlinks. The content of the element is what is displayed and the value of the href attribute is the address of the linked material.
```html
<a href="https://google.com"> Google.com </a>
```
<a href="https://google.com"> Google.com </a>

_______________________________________________________
## Image
Image Elements have no content specified by the user, so they only consist of the opening tag. The two attributes often associated with this tag are `src`, the 'source' attribute. This attributes specifies the path of the image file to be rendered. Secondly, the `alt`, or 'alternative text' attribute specifies the text that will be displayed by the broswer in the event that the image is not render. This can happen if the file path to the image is incorrect. The `width` and `heigth` attributes are used to specify the 2D size of the image in units of pixels.

```html
<img src="Assets/unnamed.png" alt="Doctor Who" width = "400" height="250" >
```
<img src="Assets/unnamed.png" alt="Doctor Who" width = "400" height="250" >

_______________________________________________________
## List
List elements come in two styles out of the box, ordered list, and unordered lists. The content of list elements are html elements called 'list items'. Unordered lists are rendered will bullets. The bullet character used can be stylistically adjusted using CSS. THe ordered lists are rendered with numbers. 

### Ordered_List_Element
```html
<ol>
<li> Item 1 </li>
<li> Item 2 </li>
<li> Item 3 </li>
</ol>
```
<ol>
<li> Item 1 </li>
<li> Item 2 </li>
<li> Item 3 </li>
</ol>

### Unordered_List_Element
```html
<ul>
<li> Item 1 </li>
<li> Item 2 </li>
<li> Item 3 </li>
</ul>
```
<ul>
<li> Item 1 </li>
<li> Item 2 </li>
<li> Item 3 </li>
</ul>

_______________________________________________________
## Head
Not all HTML elements translate to a visual image. Home HTML element house information used by the the website for back-end purposes. These unseen specifications are stored in the head element 

## Title
The Title element is nested within the Head element and specifies the text that appears in the browser tab for the website

## Body
The body element is the element that holds all of the other html elements that visually construct the website. Most of the elements previously listed, anchors, headers, images, etc. are all nested within the Body element.

## HTML
All html elements are nested within a single element know as the 'HTML' element. Within the opening and closing tags of the element are stored all other elements, the head, the body, and everyting within the head and body.

```html
<!DOCTYPE html>
<html>
    <head>
        <title> Tab Title for Website </title>
    </head>
    <body>
    </body>
</html>
```
_______________________________________________________
## Common Attributes
_______________________________________________________
### ID
_______________________________________________________
### Class
_______________________________________________________
### Title
_______________________________________________________
### Style

_______________________________________________________
## Open_Questions


_______________________________________________________
## References

[Mozilla Developer Documents](https://developer.mozilla.org/en-US/docs/Learn/HTML)

[W3Schools](https://www.w3schools.com/html/)
_______________________________________________________

[Top of Page](#HTML_Syntax)