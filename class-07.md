# Class 7 Reading Notes - HTML Tables, JS Constructor Functions

## HTML Chapter 6: Tables

**Tables** are information in a grid format

### Table Structure

|**Tag** | **Name** | **Additional notes on use** |
|-------------------|-----------------------|---------------|
| `<table>` | table | used to create a table |
| `<tr>` | table row | creates a new row in the table |
| `<td>` | table data | information stored in the table |
| `<th>` | table header| used to name the heading for the column or row |
| `<th scope="col">` | scope | header for column | 
| `<th scope="row">` | scope| header for row | 
| `<td colspan="#">` OR `<th colspan="#"` | column span | stretched entries across more than one column. use number to indicate # of columns |
|  `<td rowspan="#">` OR `<th rowspan="#"` | row span | stretches entries down more than one row. use number to indicate # of rows |

### Long Table Structure

|**Tag** | **Name** | **Additional notes on use** |
|-------------------|-----------------------|---------------|
| `<thead>` | headings | used to store all headings in the table |
| `<tbody>` | body | body of table |
| `<tfoot>` | footer | footer of table - store things like totals of table |


## JS & JQ Chapter 3: Functions, Methods, and Objects


### Creating an object: constructor notation
- Use keyword **new** and the object constructor to create a blank object
- You can add properties and methods to these objects

### Updating an object
- using dot notation:

call the object name then '.' then the property name then '=' and then the property value

### Creating many objects: constructor notation
1. Use functions as a template with the object's properties and methods
2. Name the function using an uppercase letter - helps remind developers to use the **new** keyword when creating object
3. Add parameters to function to set the value of a property in the object
  - methods will be the same for each object created using the function template
4. Use **this** keyword instead of object name to indicate the property or method belongs to the object that *this* function creates
  - use `;` instead of `,` like in the object literals


Example:

`function Name(param1, param2, param3) {`

` this.param1 = param1;`

` this.param2 = param2;`

` this.param3 = param3;`

` this.methodName = function() {`

`    code the method will execute` 

` };`

`};` 


Using Constructor function:

`let objectName = new ConstructorFunction('value', 'value', 'value');`


### Arrays and Objects

- Arrays are a special type of object
- You can combine arrays and objects to create complex data structures: 
  - Arrays can store a series of objects (and remember their order)
  - Objects can also hold arrays (as values of their properties)


### Built in Objects

Browsers come with a set of built-in objects:
1. Browser Object Model
2. Document Object Model (DOM)
3. Global JavaScript Objects


#### Browser Object Model
- creates a model of the browser tab or window

|**Method** | **Description** | 
|-------------------|-----------------------|
| `window.alert()` | creates dialog box with message (user much click okay to close it) | 
| `window.open()` | opens new browser window with url specified in parameter | 
| `window.print()` | Tells browser that user wants to print contents of current page | 


#### Document Object Model
- creates a model of the current web page

|**Method** | **Description** | 
|-------------------|-----------------------|
| `document.write()` | writes text to document | 
| `document.getElementId()` | returns element if there is an element with the value of the id | 
| `document.querySelectorAll()` | Returns list of element that match a CSS selector | 
| `document.createElement()` | creates new element | 
| `document.createTextNode()` | creates new text node | 


#### Global JavaScript Objects
- Do not form a single model... group of individual objects that relate to the JavaScript language

|**Method** | **Description** | 
|-------------------|-----------------------|
| `toUpperCase()` | Changes string to uppercase characters | 
| `toLowerCase()` | Changes string to lowercase characters | 
| `charAt()` | takes an index number as a parameter and returns the character found at that position | 
| `indexOf()` | returns index number of the first time a character is found within the string | 
| `lastIndexOf()` | returns index number of the last time a character is found within the string | 



#### More Global Objects - math and numbers

|**Method** | **Description** | 
|-------------------|-----------------------|
| `isNaN()` | checks if the value is not a number | 
| `toFixed()` | rounds to specified number of decimal places(returns a string) | 
| `toPrecision()` | Rounds to total number of places (returns a string) | 
| `toExponential()` | Returns a string representing the number in exponential notation | 
| `lastIndexOf()` | returns index number of the last time a character is found within the string |
| `Math.round()` | Rounds number (up or down) to nearest integer | 
| `Math.sqrt(n)` | returns square root of positive number | 
| `Math.ceil()` | Rounds up to the nearest integer | 
| `Math.floor()` | rounds number down to the nearest integer | 
| `Math.random()` | generates a random number between 0 and 1 |