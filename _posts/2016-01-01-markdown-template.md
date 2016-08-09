---
layout: post
title: Markdown Examples
category: Template
tags:template
---

1. Text/Emphasis
.1.1 Bold
.1.2 Italic
.1.3 BlockQuotes
.1.4 Strike-through
.1.5 Spaces
.1.6 Horizental Rules: (three or more Hyphens/Asterisks/Underscores)
.1.7 Line Breaks

2. Code and Syntax Highlighting...
3. Li/st
4. Headers
5. Links
6. Image
7. Table
8. Inline HTML
9. Emoji

1 Text/Emphasis
1.1 Bold
**This text will be bold**
__This will also be bold__

1.2 Italic
*This text will be italic*
_This will also be italic_

eg3.
_You **can** combine them_
Combined emphasis with **asterisks and _underscores_**.

1.3 BlockQuotes
As Kanye West said:

> We're living the future so
> the present is our past.
Quotes Breaks.
> Second Quots. Note here after '>', there should be a space?also, you can put **bold bold bold** or *italic italic italic* in the quotes

1.4 Strikethrough
Strikethrough uses two tildes. ~~Scratch this.~~. 

1.5 spaces
...this is a leading spaces with dots to layer out

1.6 Horizental Rules: 
Three or more...
1.6.1 Hyphens: is a line
---
1.6.2 Asterisks: is a line
***

1.6.3 Underscores: is a line
___

1.7 Line Breaks
My basic recommendation for learning how line breaks work is to experiment and discover -- hit <Enter> once (i.e., insert one newline), then hit it twice (i.e., insert two newlines), see what happens. You'll soon learn to get what you want. "Markdown Toggle" is your friend.

Here are some things to try out:

Here's a line for us to start with.

This line is separated from the one above by two newlines, so it will be a *separate paragraph*.

This line is also a separate paragraph, but...
This line is only separated by a single newline, so it's a separate line in the *same paragraph*.




2. Code and Syntax Highlighting...
Code blocks are part of the Markdown spec, but syntax highlighting isn't. However, many renderers -- like Github's and Markdown Here -- support syntax highlighting. Which languages are supported and how those language names should be written will vary from renderer to renderer. Markdown Here supports highlighting for dozens of languages (and not-really-languages, like diffs and HTTP headers); to see the complete list, and how to write the language names, see the highlight.js demo page.

Inline `code` has `back-ticks around` it.
Inline code has back-ticks around it.

Blocks of code are either fenced by lines with three back-ticks ```, or are indented with four spaces. I recommend only using the fenced code blocks -- they're easier and only they support syntax highlighting.

```javascript
var s = "JavaScript syntax highlighting";
alert(s);
```
 
```python
s = "Python syntax highlighting"
print s
```
 
```
No language indicated, so no syntax highlighting. 
But let's throw in a <b>tag</b>.
```
var s = "JavaScript syntax highlighting";
alert(s);
s = "Python syntax highlighting"
print s
No language indicated, so no syntax highlighting in Markdown Here (varies on Github). 
But let's throw in a <b>tag</b>.


3. List
3.1 Unordered List
3.1.1 Use * or + or - 
* Item 1
* Item 2
  * Item 2a
  * Item 2b

3.2 Ordered List: 
1. Item 1
2. Item 2
3. Item 3
   * Item 3a
   * Item 3b

3.3 An example 
1. First ordered list item
2. Another item
⋅⋅* Unordered sub-list. 
1. Actual numbers don't matter, just that it's a number
⋅⋅1. Ordered sub-list
4. And another item.

⋅⋅⋅You can have properly indented paragraphs within list items. Notice the blank line above, and the leading spaces (at least one, but we'll use three here to also align the raw Markdown).

⋅⋅⋅To have a line break without a paragraph, you will need to use two trailing spaces.⋅⋅
⋅⋅⋅Note that this line is separate, but within the same paragraph.⋅⋅
⋅⋅⋅(This is contrary to the typical GFM line break behaviour, where trailing spaces are not required.)

* Unordered list can use asteriskto layer outs
- Or minuses
+ Or pluses


4. Headers
4.1 method1 
# This is an <h1> tag
## This is an <h2> tag
### This is an <h3> tag
####This is an <h4> tag
##### This is an <h5> tag
###### This is an <h6> tag

4.2 method2
Alternatively, for H1 and H2, an underline-ish style:

Alt-H1
======

Alt-H2
------

5. Link: 
[this is hyperlnked text](link link title when scroll over')
or user angle brackets <put url in angle branckets>
eg. 
There are two ways to create links.

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


6. Image and Youtube Videos
6.1 Image 
Here's our logo (hover to see the title text):
6.1.1 Inline-style: 
eg1. ![GitHub Logo](/images/logo.png)

eg2. ![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 1")

6.1.2 Reference-style: 
eg1. Format: ![Alt Text](url)

eg2. ![alt text][logo]

[logo]: https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 2"

6.2 Youtube Vidoes
6.2.1 They can't be added directly but you can add an image with a link to the video like this:

<a href="http://www.youtube.com/watch?feature=player_embedded&v=YOUTUBE_VIDEO_ID_HERE
" target="_blank"><img src="http://img.youtube.com/vi/YOUTUBE_VIDEO_ID_HERE/0.jpg" 
alt="IMAGE ALT TEXT HERE" width="240" height="180" border="10" /></a>

6.2.2 
Or, in pure Markdown, but losing the image sizing and border:

[![IMAGE ALT TEXT HERE](http://img.youtube.com/vi/YOUTUBE_VIDEO_ID_HERE/0.jpg)](http://www.youtube.com/watch?v=YOUTUBE_VIDEO_ID_HERE)

Referencing a bug by #bugID in your git commit links it to the slip. For example #1.

7. Tables
You can create tables by assembling a list of words and dividing them with hyphens - (for the first row), and then separating each column with a pipe |:

eg1. 

First Header | Second Header
------------ | -------------
Content from cell 1 | Content from cell 2
Content in the first column | Content in the second column


eg2. 
Colons can be used to align columns.

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

There must be at least 3 dashes separating each header cell.
The outer pipes (|) are optional, and you don't need to make the 
raw Markdown line up prettily. You can also use inline Markdown.

Markdown | Less | Pretty
--- | --- | ---
*Still* | `renders` | **nicely**
1 | 2 | 3

8. Inline HTML
You can also use raw HTML in your Markdown, and it'll mostly work pretty well.

`<dl>
  <dt>Definition list</dt>
  <dd>Is something people use sometimes.</dd>

  <dt>Markdown in HTML</dt>
  <dd>Does *not* work **very** well. Use HTML <em>tags</em>.</dd>
</dl>

9. Emoji
Emoji Cheatsheet [http://www.webpagefx.com/tools/emoji-cheat-sheet/](http://www.webpagefx.com/tools/emoji-cheat-sheet/)


Reference: <http://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet>

Find out more by [my github](https://cwz753.github.io/lvqunbai/).
