# HTML_Syntax
[Developement Notebook](Table%20of%20Contents.md)
_______________________________________________________

## Table of Contents
**HTML_Concepts**

[HTML_Concepts](#HTML_Concepts)

**HTML_Tags**

[HTML_Tags](#HTML_Tags)

**Questions**

[Open_Questions](#Open_Questions)

**References**

[References](#References)
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
## HTML Element
_______________________________________________________
### Header Elements
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
### Paragraph Element
```html
<p> Paragraphs just look like normal test </p>
```
<p> Paragraphs just look like normal test </p>

_______________________________________________________

## Boldface Element:
The tag name for bondface elements is `strong`. It seems a strange and unintuitive thing to use, but that is just how it is unfortunately.

```html
<strong> This is how to bold something in html </strong>
```
<strong> This is how to bold something in html </strong>

_______________________________________________________

## Italic Element:
Same deal as boldface, `em` is a strange and unintuitive name to me, but that is just the way it is, sadly.

```html
<em> This is how to italicize something in html </em>
```
<em> This is how to italicize something in html </em>

_______________________________________________________

## Newline Element 
Unlike other elements so far, this one has no content and therefore only requires an opening tag.
```html
This will be a line above<br>and this will be a line below
```
This will be a line above<br> and this will be a line below

_______________________________________________________
## Image Element 
```html

```


_______________________________________________________
## Anchor Element (aka a *Link*)
```html

```
_______________________________________________________
## List Elements
List elements come in two styles out of the box, ordered list, and unordered lists. The content of list elements are html elements called 'list items'. Unordered lists are rendered will bullets. The bullet character used can be stylistically adjusted using CSS. THe ordered lists are rendered with numbers. 

### Ordered List Element
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

### Unordered List Element
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
## Open_Questions


_______________________________________________________
## References

[Mozilla Developer Documents](https://developer.mozilla.org/en-US/docs/Learn/HTML)

[W3Schools](https://www.w3schools.com/html/)
_______________________________________________________

[Top of Page](#HTML_Syntax)