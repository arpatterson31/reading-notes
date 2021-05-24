# Class 28 Reading: Component Composition

## Review, Research, and Discussion

### Can a parent component access the state of a child component?

- Yes - we can access the childs state using Refs. You can assign a Refs for the child component in the parent component. then using Refs we can access the child’s state. *[source](https://www.geeksforgeeks.org/how-to-access-childs-state-in-react/)*

### What can be passed along in a prop variable

- props can be anything!

### How can a child component "know" the state of another component?

- To obtain the state of another component, you can pass a component’s state to its child components as props. Also, you can have components share a common ancestor, and have them access the same state in a similar manner. *[source](https://discuss.codecademy.com/t/can-a-component-access-the-state-of-another-component/394157)*

## Document the following vocab words

- **component props:** “Props” is a special keyword in React, which stands for properties and is being used for passing data from one component to another. *[source](https://itnext.io/what-is-props-and-how-to-use-it-in-react-da307f500da0)*
- **component state:** is managed within the component (similar to variables declared within a function). If a Component needs to alter one of its attributes at some point in time, that attribute should be part of its state, otherwise it should just be a prop for that Component.
- **application state:** state at which an application resides with regards to where in a program is being executed and the memory that is stored for the application.*[source](https://stackoverflow.com/questions/8102674/what-is-application-state/8102688)*

## Preview

### Which 3 things had you heard about previously and now have better clarity on?

- From the 301 course I took with React, I'm familiar with setting state, passing props down to child components, and the whole this.props, vs. this.state

### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

- I was not familiar with setting Refs. This was something I discovered in the research and readings. I'd like to learn more about that. Also Hooks would be interesting to dive deeper into

### What are you most excited about trying to implement or see how it works?

- Hooks, testing, and any new tricks in React I haven't learned in 301
