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

