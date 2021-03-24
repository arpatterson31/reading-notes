# Readings: APIs

## Article - SuperAgent

- SuperAgent is a light-weight ajax API built for flexibility, readability, and a low learning curve

### Basics

 - **Request** 
  - can be made by invoking `request` object, then calling `.then()` (or `.end()` or `await`) to send the request

````javascript
request
  .get('/search')
  .then(res => {
      // res.body, res.headers, res.status
  })
  .catch(err => {
      // err.message, err.response
  });
````

- **GET** 

````javascript
request
  .get('https://example.com/search')
  .then(res => {

  });
````

- **DELETE** 
  - can be called as `.del()`

## Article Regex

- I wasn't able to read the article because I reached my free article max :(

`Audrey, read more from Jonny Fox — and everyone else on Medium.
You’ve read all your free member-only stories. Become a member to get unlimited access and support the voices you want to hear more from.`

- Regex cheatsheet:

- **Character classes**

````javascript
.	any character except newline
\w\d\s	word, digit, whitespace
\W\D\S	not word, digit, whitespace
[abc]	any of a, b, or c
[^abc]	not a, b, or c
[a-g]	character between a & g
````

- **Anchors**

````javascript
^abc$	start / end of the string
\b\B	word, not-word boundary
````

- **Escaped Characters**

````javascript
\.\*\\	escaped special characters
\t\n\r	tab, linefeed, carriage return
````

- **Groups and Lookaround**

````javascript
(abc)	capture group
\1	backreference to group #1
(?:abc)	non-capturing group
(?=abc)	positive lookahead
(?!abc)	negative lookahead
````

- **Quantifiers and Alternation**

````javascript
a*a+a?	0 or more, 1 or more, 0 or 1
a{5}a{2,}	exactly five, two or more
a{1,3}	between one & three
a+?a{2,}?	match as few as possible
ab|cd	match ab or cd
````

