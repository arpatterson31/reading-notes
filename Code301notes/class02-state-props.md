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
