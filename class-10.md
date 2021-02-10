# Class 10 - JS Debugging

JS Chapter 10: "Error Handling & Debugging"

JavaScript is hard to learn and no one's code is perfect the first time it's written! (First hand experience here...)

There are ways and tools to help you find errors in your code. 

### Execution used with debugging

Order
- The order in which statements are executed are complex; some tasks cannot complete until another statement or function has been run. 


Contexts
- Every statement in a script lives in one of three execution contexts
	- Global Context 
	- function context
	- eval context
- Variable Scope 
	- Global Scope
	- Function-Level Scope


### Error Objects

Error Objects can help you find where your mistakes are and browsers have tools to help you read them


Properties of an Error Object

|**Property** | **Description** | 
|-------------------|-----------------------|
| `name` | type of error | 
| `message` | Description | 
| `fileNumber` | name of the javascript file | 
| `lineNumber` | line number of error | 


Types of Error Objects

|**Object** | **Description** | 
|-------------------|-----------------------|
| `Error` | Generic error - the other errors are all based on this error | 
| `SyntaxError` | Syntax has not been followed | 
| `ReferenceError` | Tried to reference a variable that is not declared/within scope | 
| `TypeError` | An unexpected data type that cannot be coerced | 
| `RangeError` | Numbers not in a acceptable range | 
| `URIError` | encodeURI(), decodeURI(), similar methods used incorrectly | 
| `EvalError` | eval() function used incorrectly | 


### Handling Errors

1. Debug the script to fix errors
	1. Where is the problem
	2. What exactly is the problem
2. Handle errors gracefully

### Console methods
There are more than just console.log!

- `console.info()` - can be used for general information
- `console.warn()` - can be used for warnings
- `console.error()` - can be used to hold errors
- `console.group()` - groups messages together
- `console.table()` - outputs a table showing objects and arrays
- `console.assert()` - test if a condition is met and write to the console only if evaluates to false


### Breakpoints
- You can pause the execution of a script on any line using breakpoints. 

- You can set multiple breakpoints and step through them one by one to see were a problem might occur

- Conditional breakpoints can be used to if a condition you specify is met