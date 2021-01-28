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
