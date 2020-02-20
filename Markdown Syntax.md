## **Markdown Syntax**
---

## *Headers:*

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

```bash
*Italics*
_Italics_
```
*Italics* <br>
_Italics_

---

## *Boldface:*
```bash
**Boldface**
__Boldface__
```
**Boldface** <br>
__Boldface__

---

## *Strikethrough:*
```bash
~~Strikethrough~~
```
~~Strikethrough~~

---

## *Tables:*
Colons can be used to align columns.
```bash
| Header 1      | Header 2      | Header 3      |
| ------------- |:-------------:| -------------:|
| left-algined  |center-aligned | right-aligned |

```

| Header 1      | Header 2      | Header 3      |
| ------------- |:-------------:| -------------:|
| left-algined  |center-aligned | right-aligned |

<br>

---

## *Block Quotes:*
```bash
> This is a block quote. There should be a vertical line to the left
```
> This is a block quote. There should be a vertical line to the left

---

## *Ordered Lists:*
```bash
1. List Item 1
2. List Item 2
3. List Item 3
```
1. List Item 1
2. List Item 2
3. List Item 3

---

## *Unordered Lists:*
```bash
- List Item 1
- List Item 2
- List Item 3
```
- List Item 1
- List Item 2
- List Item 3

---

## *Code Quotes:*
```markdown
The code in the `backticks` will be formatted distinctly
```

The code in the `backticks` will be formatted distinctly

---

## *Fenced Code Blocks:*
Using three backticks will create a Fenced Code Block. You can add a specifying keyword to describe the code language being used and special highlightling rules may apply.
```bash
```bash
Take out the escape backslash and this will render a code block 
\```
```
```bash
Take out the escape backslash and this will render a code block 
```

---

## *Links:*
Links can be created a variety of ways in Markdown. <br>
Typing out a web address automatically creates a link.
```
http://github.com
```
http://github.com<br>

The next method creates a link to the address in parentheses and displays the content in the square brackets
```
[GitHub](http://github.com)
```

[GitHub](http://github.com)

---

## *Images:*
```bash
```

---

## *Task Lists:*
```bash
- [ ] Open Task Item
- [X] Closed Task Item
```

- [ ] Open Task Item
- [X] Closed Task Item

---

## *Backslash Escapes:*
Any character preceeded by a backslash will be rendered as a regular character.

```bash
With a backslash this \`code\` quote will not work.

```
With a backslash this \`code\` quote will not work

---

## *Lines Across*

```markdown
---
```

---
<br>

---

## *References*

[Adam-P Notes](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet#links)

---
<br>
<br>
<br>

## **Sourced Notes - To Be Reformatted**

## *Link Notes*

[I'm an inline-style link](https://www.google.com)

[I'm an inline-style link with title](https://www.google.com "Google's Homepage")

[I'm a reference-style link][Arbitrary case-insensitive reference text]

[I'm a relative reference to a repository file](../blob/master/LICENSE)

[You can use numbers for reference-style link definitions][1]

Or leave it empty and use the [link text itself].

URLs and URLs in angle brackets will automatically get turned into links. 
http://www.example.com or <http://www.example.com> and sometimes 
example.com (but not on Github, for example).

Some text to show that the reference links can follow later.

[arbitrary case-insensitive reference text]: https://www.mozilla.org
[1]: http://slashdot.org
[link text itself]: http://www.reddit.com

when using local reference links, the space character is not supported. Trying using file names without spaces, or use "%20" in place of a space character in the markdown link


-----

## *Image Notes*

Here's our logo (hover to see the title text):

Inline-style: 
![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 1")

Reference-style: 
![alt text][logo]

[logo]: https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 2"
Here's our logo (hover to see the title text):

Inline-style: alt text

Reference-style: alt text