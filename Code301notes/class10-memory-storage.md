# Readings: In Memory Storage

## Article - The JavaScript Call Stack - What it is and why it's necessary

- JavaScript engine is a single-threaded interpreter comprising of a heap and a single call stack
- browswers provides web APIs like the DOM, AJAX, and Timers

- **Call Stack** - used for function calls
  - a data structure
  - used Last In, First Out principle to store and manage function calls
  - last function that gets pushed into the stack is the first to be popped out

- **Asynchronous JS** - a callback function, an event loop, and a task queue
  - callback function is acted upon by the call stack

### Example of a LIFO

````javascript
function firstFunction(){
  throw new Error('Stack Trace Error');
}

function secondFunction(){
  firstFunction();
}

function thirdFunction(){
  secondFunction();
}

thirdFunction();
````

- Above example gives an error 

### Manage function invocation

- Call stack maintains a record of the position of each stack frame

- **Stack Overflow** occurs when there is a recursive function (a function that calls itself) without an exit point

## Article - JavaScript error messages && debugging

### Types of error messages

- Reference errors
  - ie variable is not yet declared
- Syntax errors
  - missing semicolon!!
- Range errors
  - manipulating an obj with some kind of length that doesn't exist
- Type error
  - types (number, string...) aren't compatible

### Debugging

- easiest way to debug is the `console.log()`
- could also use conditional breakpoints

### Handling Errors

- try and catch methods are great!