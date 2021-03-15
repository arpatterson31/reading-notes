# Readings: State and Props

## Article - React - State and Lifecycle

## Article - React - Handling Events

- Handling events with React are similar to handling events on DOM elements
  - React events are named using camelCase rather than lowercase
  - With JSX you pass a function as the event handler, rather than a string
  - you must call `preventDefault` to prevent default behavior in React
  
### Example Code

````javascript
<button onclick={activateLasers}>
  Activate Lasers
</button>
````

- You generally don't need to call `addEventListener` when using React
  - instead provide a listener when the element is initially rendered

### Passing Arguments to Event Handlers

- `Arrow functions` and `Function.prototype.bind` can be used to pass arguments to Event Handlers

## Article - Conditional Rendering

- React allows you to create distinct components that uses behaviors you need, then render only some of them, depending on the state of your application

- Works the same as in JavaScript
  - use `if` or the `conditional operator` to create elements 

### Example code

````javascript
function Greeting(props) {
  const isLoggedIn = props.isLoggedIn;
  if (isLoggedIn) {
    return <UserGreeting />;
  }
  return <GuestGreeting />;
}

ReactDOM.render(
  <Greeting isLoggedIn={false} />,
  document.getElementById('root')
);
````

### Element Variables

- variables can store elements

### Conditional Rendering

- If with Logical `&&` Operator
  - `true && expression` always evaluates to `expression`
  - `false && expression` always evaluates to `false`
  - `falsy` will always be skipped but will return the falsy expression

- If-Else with Conditional Operator
  - `condition ? true : false`

### Preventing Component from Rendering

- return `null` instead of render output
