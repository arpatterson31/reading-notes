# Readings: Passing Functions as Props

## Article - Lifting State Up

- When components need to reflect the same changing data, lifting the shared state up to their closest common parent will work

- Changing state
  - declaring state prop in the constructor
  - then using `this.setState();` to update the prop

- Sharing state is accomplished by moving it up to the closest common parent of the components that need it.
  - also referred to as "lifting state up"
  - rely on "top-down data flow"

## Article - List and Keys

### Rendering Multiple Components

- Use `.map()` to loop through the array to return elements for each item
  - It's important that a key should be provided for each element
