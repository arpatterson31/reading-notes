# Readings: Introduction to React and Components

## Article - React Tutorial through 'Passing Data Through Props'

### Vocab

- **REACT**  a JavaScript library for building user interfaces
- **components**  small and isolated pieces of code used in React to write complex UIs -- we used components to tell React what we want to see on the screen.  When data changes, React will update and re-render components.
- **props**  short for properties -- components takes in parameters called props
- **render** method to return what you want to see on the screen
- **JSX**  a special syntax used to write render structures

- Passing props is how info flows in React apps, from parents to children
- To "remember" things, componets use **state**
  - this.state set in constructors -- private to the component it is defined in

## Article - Hello World - React

- Building blocks of React apps: elements and components

- Move over `console.log(hello, world!)` there is a new proof of life in town!

```` javascript

ReactDOM.render(
  <h1>Hello, world!</h1>,
  document.getElementById('root')
);
````

## Article - Introducing JSX - React

- JSX is a syntax extension to JavaScript
- JSX produces React "elements"
- JSX isn't required but it is helpful when needing a visual aid when working with UI inside of JavaScript code
- JSX allows React to show more useful error and warning messages

### Example code

````javascript
const name = 'Audrey';
const element = <h1>Hey, {name}</h1>;

ReactDOM.render(
  element,
  document.getElementById('root')
);
````

- Any valid JavaScript expressions can be put inside curly braces in JSX
  - curly braces for expressions
  - quotes for string values
- JSX is an expression too and can be used in function calls and objects
  - can be used inside of `if` statements and `for` loops
- JSX tags can contain children like `li` in an `ul`
- JSX can also represent Objects using the `React.createElement()`;

## Article - Rendering Elements

- Elements are the smallest building blocks of React apps.
  - describes what you want to see on the screen

- DOM nodes get an id of "root" because everything inside it will be managed by React DOM

- To render a React element to the root DOM, you'd pass both to `ReactDom.render();`
  
````javascript
const element = <h1>Hey, girl hey!</h1>;
ReactDOM.render(element, document.getElementById('root'));
````

- Elements are unchangeable. Once you create an element, you can't change its children or attributes.
  - to update the UI, create a new element and pass it

## Article - Components and Props

