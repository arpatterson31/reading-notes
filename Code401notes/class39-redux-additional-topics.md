# Class 39 Reading: Redux - Additional Topics

## Review, Research, and Discussion

### What's the best practice for "pre-loading" data into the store (on application start) in a Redux application?

- The most 'redux-like' way of handling the pre-loading of data would be to fire off the asynchronous action in the lifecycle method (probably useEffet) of a Higher Order Component that wraps your app. However, you will not use the results of the API call directly in that component - it needs to be handled with a reducer that puts it into your app store. This will require you to use some sort of a thunk middleware to handle the asynchronous action. Then you will use mapStateToProps to simply pass it down to the component that renders the data. *[source](https://stackoverflow.com/questions/39356517/correct-way-to-pre-load-component-data-in-reactredux)*

### When using a thunk/async action that dispatches the actual action, which do you export from your reducer?

- You'd export your action creator *[source](https://medium.com/@stowball/a-dummys-guide-to-redux-and-thunk-in-react-d8904a7005d3)*

## Document the following vocab words

- **middleware:** function that takes the req, changes/does something to it and then passes next
- **thunk:** middleware that allows you to return functions, rather than just actions, within Redux. This allows for delayed actions, including working with promises. *[source](https://www.freecodecamp.org/news/redux-thunk-explained-with-examples/)*

## Preview

### Which 3 things had you heard about previously and now have better clarity on?

- The redux toolkit, mobx are new concepts. I haven't heard or used them previously.

### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

- The toolkit, and MobX

### What are you most excited about trying to implement or see how it works?

- More on the thunk and async functions in redux
