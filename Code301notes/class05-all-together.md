# Readings: Putting it all together

## Article - Thinking in React

### Wireframe/UI

- Wireframes for a React is more of breaking the UI into a component hierarchy
  - draw boxes around every component and subcomponent and give them names

- **Single responsibility principle:** a component should ideally only do one thing
  - If it grows, it should be decomposed into smaller subcomponents

### Getting started with a static app

- Building a static app will be the easiest way but includes no interactivity
  - Build components that reuse other components and pass data using props
  - Don't use state at all during a static build
  - Build top down OR bottom up

### Adding Interactivity

- **State** is what makes your app interactive as it changes the data

- Figuring out what component should hold state:
  - Identify every component that renders something based on that state.
  - Find a common owner component (a single component above all the components that need the state in the hierarchy).
  - Either the common owner or another component higher up in the hierarchy should own the state.
  - If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.
