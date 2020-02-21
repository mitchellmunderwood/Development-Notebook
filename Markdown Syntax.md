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

## *Block Quotes:*
```
> This is a block quote. There should be a vertical line to the left.
```
> This is a block quote. There should be a vertical line to the left.

---

## *Ordered Lists:*
```
1. List Item 1
2. List Item 2
3. List Item 3
```
1. List Item 1
2. List Item 2
3. List Item 3

---

## *Unordered Lists:*
```
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
The code in the `backticks` will be formatted distinctly.
```

The code in the `backticks` will be formatted distinctly.

---

## *Fenced Code Blocks:*
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

## *Links:*
Links can be created a variety of ways in Markdown. <br>
Typing out a web address automatically creates a link.
```
http://github.com
```
http://github.com<br>

The next method creates a link to the address in parentheses and displays the content in the square brackets.
```
[GitHub](http://github.com)
```

[GitHub](http://github.com)

---

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

## *Task Lists:*
```
- [ ] Open Task Item
- [X] Closed Task Item
```

- [ ] Open Task Item
- [X] Closed Task Item

---

## *Backslash Escapes:*
Any character preceeded by a backslash will be rendered as a regular character.

```
With a backslash this \`code\` quote will not work.
```
With a backslash this \`code\` quote will not work.

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

