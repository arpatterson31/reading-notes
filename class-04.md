# Class 4 Reading Notes - HTML Links, JS Functions, and Intro to CSS Layout

## Links

**Links** allow you to move from one page/place to another - browsing the web

Types of Links

- One website to another
- from one page to another on the same website
- from one part of the page to another but on the same page
- ones that open into a new browser window
- ones that start up another program like your email

Links are created using an anchor tag: `<a></a>`

How to write links:

- Linking to another website: `<a href="url that you want the link to take you to">TEXT</a>`
- other page on same site: `<a href="index.html">TEXT</a>`
  - for pages in folders or directories, make sure to reference the folder structure
- Email Links: `<a href="mailto:name@example.com">EMAIL</a>`
- Open new window: `<a href="www.url.com" target="_blank">TEXT</a>`


## Layout

### Core Concepts

CSS treats each HTML element like it's in its own box

Boxes will either be **block-level** or **inline**


**Block-Level**
start on a new line and act as main building block of layout
examples of block-level: `<h1>` or `<p>` or `<li>`


**Inline**
these boxes flow between surrounding text
examples of inline: `<b>` or `<img>` or `<i>`


If block-level elements sit in another block element you can group them together using a `<div>` tag


### CSS Positioning Schemes

- Normal Flow
  - every block appears on the same line
- Relative Positioning
  - shifts element to Top, Left, Right, or bottom of where it was originally placed
- Absolute Positioning
  - positions the element in relation to its containing element
- Fixed Positioning
  - positions the element in relation to the browser window
- Floating Elements
  - takes it out of its normal position and moves it to the far right or far left



## Functions, Methods, and Objects
