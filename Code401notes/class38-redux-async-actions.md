# Class 38 Reading: Redux - Asynchronous Actions

## Review, Research, and Discussion

### How granular should your reducers be?

- It should be as granular as you can be. This typically leads to better UI performance, as fewer components will need to render when a given piece of state changes. *[source](https://redux.js.org/style-guide/style-guide)*

### Pro or Con - multiple reducers can "fire" when a commonly named action is dispatched

- This is a con, you should avoid dispatching several times synchronously in a row in the places where you're concerned about performance. There are a number of addons and approaches that can batch up dispatches as well. *[source](https://redux.js.org/faq/actions#should-i-dispatch-multiple-actions-in-a-row-from-one-action-creator)*

### Name a strategy for preventing the above

- If you actually are concerned about reducer performance, you can use a utility such as redux-ignore or reduxr-scoped-reducer to ensure that only certain reducers listen to specific actions. You can also use redux-log-slow-reducers to do some performance benchmarking. *[source](https://redux.js.org/faq/performance#wont-calling-all-my-reducers-for-each-action-be-slow)*

## Document the following vocab words

- **store:** a single object tree that contains the state of the app
- **combined reducers:** helper function turns an object whose values are different reducing functions into a single reducing function you can pass to `createStore`.

## Preview

### Which 3 things had you heard about previously and now have better clarity on?

- I'm familiar with async actions but not in relation to redux..hopefully it isn't that much different

### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

- Thunk is a new term/concept for me so I'm interested in learning more about that

### What are you most excited about trying to implement or see how it works?

- Thunk, more async actions and more on redux
