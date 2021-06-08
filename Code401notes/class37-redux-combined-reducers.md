# Class 37 Reading: Redux - Combined Reducers

## Review, Research, and Discussion

### Why choose Redux instead of the Context API for global state?

- Redux works around the idea of having a central state called a store. To change the state, a component has to dispatch an action. The action is then passed on to the reducer, which changes the state of our application. *[source](https://betterprogramming.pub/why-use-redux-when-we-have-context-api-95be70581148)*

### What is the purpose of a reducer?

- A reducer is a function that evaluates the type of action and creates a new copy of state

### What does an action contain?

- An object literal that contains a type and a payload

### Why do we need to copy the state in a reducer?

- Reducers must always follow some special rules:
  - They should only calculate the new state value based on the state and action arguments
  - They are not allowed to modify the existing state. Instead, they must make immutable updates, by copying the existing state and making changes to the copied values.
  - They must not do any asynchronous logic or other "side effects"

## Document the following vocab words

- **immutable state:** state that can't be changed
- **time travel in redux:** you can see the "state" of state at particular times in the lifecycle or renderings without having to restart or reload the app
- **action creator:** function that returns an action
- **reducer:** function that evaluates the type of action and creates a new copy of state
- **dispatch:** happens in the component level and this triggers the state change

## Preview

### Which 3 things had you heard about previously and now have better clarity on?

- the combined reducer and multiple reducers as we are currently using those in lab

### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

- Need more info on this redux, it's tricky and a little confusing and easy to get lost in

### What are you most excited about trying to implement or see how it works?

- More of the material UI and deeper into redux
