# Class 9 Reading Notes - Forms and JS Events

## HTML Chapter 7: Forms

HTML can create forms to collect information from visitors to your site. 


### Form Controls:
- Adding text
  - text input - single line or multi-line
  - password input
- making choices
  - radio buttons - user must select one of a number of options
  - checkboxes - user can select and unselect one or more options
  - drop-down boxes - user must pick one of a number of options from a list
- submitting forms
  - submit buttons
  - image buttons - similar to submit but allows you to use an image 
- uploading files
  - file upload


### How Forms work

1. user fills in a form and presses a button to submit the info to the server
2. the name of each form control is sent to the server along with the value the user entered
3. server processes the information using a programming language
4. server creates a new page to send back to the browser based on the information received


### HTML Structure

`<form>`

`action` - every form requires an action. It's value is the URL for the page on the server that will receive the info in the form when it is submitted

`method` - get or post - form can be sent using on of those 2 methods

- get method examples: search boxes or short forms
- post method examples: uploading files, or contains sensitive data like passwords, or adds info to a database


`<form action="https://www.url.com" method="get"></form>`


### HTML Structure for Form controls

1. Text Input

`<input type="text" name="" maxlength="" />`

- name: value of this identifies the form control and is sent along with the info they enter to the server
- maxlength: limit the number of characters a user may enter into the field

2. Password Input

`<input type="password" name="" maxlength="" />`

3. Text Area

`<text area name="" cols="" rows=""></textarea>`

4. Radio Button

`<input type="radio" name="" value="" checked="checked" />`

- create a tag for each button but only one will have a checked attribute

5. Checkbox

`<input type="checkbox" name="" value="" checked="checked" />`

6. Drop down list

`<select name="">`

`<option value=""></option>`

`</select>`

- create a tag for each option

7. Mutltiple Select box

`<select name="" size="" multiple="multiple">`

`<option value="" selected=""></option>`

`</select>`

8. File Input box

`<input type="file" name="" />`

`<input type="submit" value="upload" />`

9. Submit button

`<input type="submit" name="" value="" />`

10. Image button

`<input type="image" src="" width="" height="" />`


- Grouping Form Elements

`<fieldset>`

`<legend>`

`<input>`

`<input>`

`</fieldset>`

### Additional Input Types for HTML5

- date 
- email 
- url
- search


## HTML Chapter 14: List, Tables & Forms

### Using CSS to style lists

`list-style-type:`


- unordered lists
  - none
  - disc
  - circle
  - square

- ordered lists
  - decimal:  1 2 3
  - decimal-leading-zero: 01 02 03
  - lower-alpha: a b c
  - upper-alpha: A B C
  - lower-roman: i. ii. iii.
  - upper-roman: I II III


`list-style-image: url("images/star.png");`


### Using CSS to style tables

- many learned properties at this point can help to style tables like padding, spacing, text-align


### Using CSS to style forms

- CSS can help make forms easier to use and can make them feel more interactive



## JS Chapter 6: Events

**Events** happen when a user clicks or taps on a link, hover or swipe over an element, type on a keyboard, resize the window, or when the page they requested loads.


### Different Event types

- UI Events 
  - load: web page finished loading
  - unload: web page is unloading
  - error: browser encounters a JS error
  - resize: window has been resized
  - scroll: user scrolled up or down the page

- Keyboard Events
  - keydown: user first presses a key
  - keyup: user releases a key

- Mouse Events
  - click: user presses and releases a button over the same element
  - dblclick: user double clicks
  - mousedown: user presses a mouse button while over an element
  - mouseup: user releases a mouse button while over an element
  - mousemove: user moves the mouse
  - mouseover: user moves the mouse over an element
  - mouseout: user moves the mouse off an element

- Form Events
  - input
  - change
  - submit
  - reset
  - cut
  - copy
  - paste
  - select



### JavaScript and Events

- Events can trigger a function - this changes the website and makes it feel interactive becasue it has responded to the user

