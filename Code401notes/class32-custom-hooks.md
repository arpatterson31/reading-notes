# Class 32 Reading: Custom Hooks

## Review, Research, and Discussion

### What does a component's lifecycle refer to?

- Each component in React has a lifecycle which you can monitor and manipulate during its three main phases. The three phases are: Mounting, Updating, and Unmounting. *[source](https://www.w3schools.com/react/react_lifecycle.asp)*

### Why do you sometimes need to "wrap" functions in useCallback when called from within useEffect?

- It's used to prevent an infinite loop. By wrapping it around a function declaration and defining the dependencies of the function, it ensures that the function is only re-created if its dependencies changed. Hence the function is NOT re-built on every render cycle anymore. You break out of the infinite loop! *[source](https://medium.com/@infinitypaul/reactjs-useeffect-usecallback-simplified-91e69fb0e7a3#:~:text=useCallback()%20helps%20you%20prevent,out%20of%20the%20infinite%20loop!)*

### Why are functional components preferred over class components?

- Functional component are much easier to read and test because they are plain JavaScript functions without state or lifecycle-hooks. You end up with less code. They help you to use best practices. *[source](https://djoech.medium.com/functional-vs-class-components-in-react-231e3fbd7108#:~:text=Functional%20component%20are%20much%20easier,you%20to%20use%20best%20practices.)*

### What is wrong with the following code?

````javascript
import React, {useState, useEffect} from 'react';

function MyComponent(props) {
  const [count, setCount] = useState(0);

  function changeCount(e) {
    setCount(e.target.value);
  }

  let renderedItems = []

  for (let i = 0; i < count; i++) {
    useEffect( () => {
      console.log('component mount/update');
    }, [count]);

    renderedItems.push(<div key={i}>Item</div>);
  }

  return (<div>
     <input type='number' value={count} onChange={changeCount}/>
      {renderedItems}
    </div>);
}
````

- The useEffect will cause an infinite loop without being wrapped in a useCallback

## Document the following vocab words

- **state hook:** a Hook that lets you add React state to function components. *[source](https://reactjs.org/docs/hooks-state.html)*
- **effect hook:** lets you perform side effects in function components. Data fetching, setting up a subscription, and manually changing the DOM in React components are all examples of side effects. Whether or not you’re used to calling these operations “side effects” (or just “effects”), you’ve likely performed them in your components before. *[source](https://reactjs.org/docs/hooks-effect.html)*
- **reducer hook:** An alternative to `useState`. Accepts a reducer of type `(state, action) => newState`, and returns the current state paired with a dispatch method.  `useReducer` is usually preferable to `useState` when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one. `useReducer` also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks. *[source](https://reactjs.org/docs/hooks-reference.html#usereducer)*

## Preview

### Which 3 things had you heard about previously and now have better clarity on?

- functional components, lifecycles

### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

- More on the hooks and the useEffect and useCallback. I also want more info on functional components even though I've heard of them previously

### What are you most excited about trying to implement or see how it works?

- The hooks!
