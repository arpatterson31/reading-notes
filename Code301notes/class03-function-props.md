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

#### Keys

- **key** is a special string attribute you need when creating lists of elements
- Keys help React identify which items have changed, are added, or are removed
- Keys give elements a stable identity
- If you don't have keys, you could use the item index as a last resort but could break if order changes
- Keys must be unique among siblings but could used the same key in different arrays

- Embed expression in curly brace so you could inline `map()`

## Tutorial - Up to Declaring a Winner

- To collect data from multiple children or to have child components communicate with each other, you have to declare the shared state in their parent component
- Parent can then pass the state back down using `props`



## Article - The Spread Operator

- The spread operator can add items to arrays, combine arrays or objects, and spread an array out into a function's argument

- Spread syntax is an ellipsis of three dots or `...`

### Code Examples

````javascript
Math.max(1,3,5) // returns the largest number - 5
Math.max([1,3,5]) // returns NAN because it expects separate arguments
````

- Using `...`

````javascript
Math.max(...[1,3,5]) // returns 5 because it spreads the array into sep arguments
````

### Uses

- Copying an array
- Concatenating or combining arrays
- Using Math functions
- Using an array as an argument
- Adding an item to a list
- Adding to state in React
- Combinging Objects
- Converting NodeList to an array

### Example for adding to state in React

````javascript
function App() {
  // React Hooks declarations
  const [searches, setSearches] = useState([])
  const [query, setQuery] = useState("")

  const handleClick = () => {
    // Add the search term to the list onClick of Search button
    // (Actually searching would require an API call here)

    // Save search term state to React Hooks
    setSearches(searches => [...searches, query])
  }
  ````

### To note

- The Spread Operator only effects the first level, not any deeply nested arrays/objects

