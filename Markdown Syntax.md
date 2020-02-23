# **Markdown Syntax**
[Development Notebook](Table%20of%20Contents.md)

---
## Table of Contents
[Header](<#Headers>) <br>
[Italics](#Italics) <br>
[Boldface](#Boldface) <br>
[Strikethrough](#Strikethrough) <br>
[Tables](#Tables) <br>
[Block_Quotes](#Block_Quotes) <br>
[Ordered_Lists](#Ordered_Lists) <br>
[Unordered_Lists](#Unordered_Lists) <br>
[Code_Quotes](#Code_Quotes) <br>
[Fenced_Code_Blocks](#Fenced_Code_Blocks>) <br>
[External_Links](#External_Links) <br>
[Internal_Links](#Internal_Links) <br>
[Images](#Images) <br>
[Task_Lists](#Task_Lists) <br>
[Backslash_Escapes](#Backslash_Escapes) <br>
[Lines_Across](#Lines_Across) <br>
[New_Lines](#New_lines) <br>
[References](#References) <br>

---
## *Headers:*
<a name="Header"></a>
```
## Header 1
### Header 2
#### Header 3
```
# Header 1
## Header 2
### Header 3

```
#### Header 4
##### Header 5
###### Header 6
```
#### Header 4
##### Header 5
###### Header 6

---

## *Italics:*

```
*Italics*
_Italics_
```
*Italics* <br>
_Italics_

---

## *Boldface:*
```
**Boldface**
__Boldface__
```
**Boldface** <br>
__Boldface__

---

## *Strikethrough:*
```
~~Strikethrough~~
```
~~Strikethrough~~

---

## *Tables:*
A combination of colons and dashes is used to assign alignment.
```
| Header 1      | Header 2      | Header 3      |
| :--           |      :-:      |            --:|
| left-algined  |center-aligned | right-aligned |

```

| Header 1      | Header 2      | Header 3      |
| :-- |:-:| --:|
| left-algined  |center-aligned | right-aligned |

<br>

---

## *Block_Quotes:*
```
> This is a block quote. There should be a vertical line to the left.
```
> This is a block quote. There should be a vertical line to the left.

---

## *Ordered_Lists:*
```
1. List Item 1
2. List Item 2
3. List Item 3
```
1. List Item 1
2. List Item 2
3. List Item 3

---

## *Unordered_Lists:*
```
- List Item 1
- List Item 2
- List Item 3
```
- List Item 1
- List Item 2
- List Item 3

---

## *Code_Quotes:*
```markdown
The code in the `backticks` will be formatted distinctly.
```

The code in the `backticks` will be formatted distinctly.

---

## *Fenced_Code_Blocks:*
Using three backticks will create a Fenced Code Block. You can add a specifying keyword to describe the code language being used and special highlightling rules may apply.
```
\```
Take out the escape backslashes and this will render a code block. 
\```
```
```
This will render a code block. 
```

---

## *External_Links:*
Links can be created a variety of ways in Markdown. <br>

When using local reference links, the space character may not be supported. Trying using file names without spaces, or use "%20" in place of a space character in the markdown link. Github does not support links using the "%20" tactic.


```
http://github.com
```
http://github.com<br>

```
[GitHub](http://github.com)
```

[GitHub](http://github.com)

```
[This is an inline-style link](https://www.google.com)
```
[This is an inline-style link](https://www.google.com)

```
[This is an inline-style link with a title](https://www.google.com "Google URL")
```
[This is an inline-style link with a title](https://www.google.com "Google URL")

```
[This is a relative reference to a repo file](/Git%20Syntax.md)
```
[This is a relative reference to a repo file](/Git%20Syntax.md)

```
[This is a reference-style link][reference text]
[reference text]: https://www.mymerrill.com
```
[This is a reference-style link][reference text]

```
[You can use numbers for reference-style link definitions][1]
[1]: http://chase.com
```
[You can use numbers for reference-style link definitions][1]

```
Or use the [reference text].
```
Or use the [reference text].

```
URLs and URLs in angle brackets will automatically get turned into links. 
http://www.example.com or <http://www.example.com>.
```
URLs and URLs in angle brackets will automatically get turned into links. 
http://www.website.com or <http://www.website.com>.

[reference text]: https://www.mymerrill.com
[1]: http://chase.com

---
## *Internal_Links:* 
Internal Links can be created to route to different parts of the markdown file by using the bracket & parenthesis notation, puting the link content in the brackets, and the link address in the parentheses. The link address will be the characters that would normally signify a header, but markdown will process this as a link to the header with the same name as that specified.
```
[Header](#Headers) 
```
[Header](#Headers)
___


## *Images:*

Inline Style
```
![alt text](https://pupsterpassion.com/wp-content/uploads/2019/10/cute-puppy.png "Call of the Wild")
```

![alt text](https://pupsterpassion.com/wp-content/uploads/2019/10/cute-puppy.png "Call of the Wild")

Reference Style
```
![alt text][logo]

[logo]: https://pupsterpassion.com/wp-content/uploads/2019/10/cute-puppy.png "Call of the Wild"
```
![alt text][logo]

[logo]: https://pupsterpassion.com/wp-content/uploads/2019/10/cute-puppy.png "Call of the Wild"


---

## *Task_Lists:*
```
- [ ] Open Task Item
- [X] Closed Task Item
```

- [ ] Open Task Item
- [X] Closed Task Item

---

## *Backslash_Escapes:*
Any character preceeded by a backslash will be rendered as a regular character.

```
With a backslash this \`code\` quote will not work.
```
With a backslash this \`code\` quote will not work.

---

## *Lines_Across*
Using 3 Dashes

```
---
```

---
<br>

Using 3 Underscores
```
___
```

___

<br>

---

## *New_Lines*
The page break operator from HTML is supported in markdown. Just add at the end of a line of code or drop down to a new line and then add.
```
This text will be <br> on the next line
```
This text will be <br> on the next line

___

## *References*

[Adam-P Notes](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet#links) <br>
[Markdown Monster Documentation](https://markdownmonster.west-wind.com/docs/_4xs10gaui.htm) <br>
[CommonMark Specs for Markdown rendered in Github](https://spec.commonmark.org/0.27/)
---


