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
