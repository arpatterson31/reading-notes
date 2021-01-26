# Class 6 Reading Notes - Problem Domain, Objects, and the DOM

## Object Literals

Objects group variables and functions and give them new names

- Variables become known as properties
- Functions become known as methods

- Properties tell us about the object and Methods represents the task that are associated with the object.

### Creating an Object Literal

`// Set up the object`

`var hotel = {`

  `name : 'Park',`

  `rooms : 120,`

  `booked : 77,`

  `checkAvailability : function() {`

  `  return this.rooms - this.booked; // Need "this" because inside function`

 ` }`

`};`



#### Accessing an object

`var hotelName = object['property name'];`

`var hotelName = object['method name']();`


## Document Object Model

*The Document Object Model specifies how browsers should create a model of an HTML page and how JS can access and update the content of a web page.*


**DOM tree** is the structure of the model 

Consists of 4 types of nodes:
- Document 
- Element 
- Attribute
- Text

![DOM tree model example from w3schools:](https://www.w3schools.com/js/pic_htmltree.gif)


### Accessing DOM Tree

- Locate the node that represents the element you want to work with
  - `getElementById()`
  - `getElementByClassName()`
  - `parentNode`
- Use its text content, child elements, and attributes

- Accessing ELEMENTS (these go in parentheses)
  - id
  - css selector ('li.nameOfListItem')
  - class 
  - tagName

### NodeLists
*DOM method can return more than one element, it returns a NodeList*


Selecting elements from NodeList
- item()METHOD
- Array Syntax

Can loop through NodeList

### Traversing the DOM

- parentNode
- previousSibling
- nextSibling
- firstChild
- lastChild

### Access & Update a text Node
- Use nodeValue property


## Adding to DOM
- createElement()
- createTextNode()
- appendChild()

## Removing Element from DOM
- removeEl
- removeChild()

## Techniques for adding HTML to web page
- document.write()
- element.innerHTML