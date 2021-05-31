# Class 33 Reading: Context API

## Review, Research, and Discussion

### Describe use cases for useMemo() and useReducer()?

- `useMemo()`: You're noticing a component's render is frustratingly slow, and you're passing a calculation to an unknowable number of children, such as when rendering children using Array.map()... or Your app often becomes unresponsive because you're fetching a large amount of data, and having to transform it into a usable format *[source](https://maxrozen.com/understanding-when-use-usememo)*

- `useReducer()` is usually preferable to `useState` when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one. `useReducer` also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks. *[source](https://reactjs.org/docs/hooks-reference.html#usereducer)*

### Why do custom hooks need the use prefix?

- So that you can tell at a glance that the rules of Hooks apply to it. *[source](https://reactjs.org/docs/hooks-custom.html)*

### What do custom hooks usually do?

- Custom hooks allow us to have cleaner functional components, remove logic from the UI layer, and prevent code duplication by bringing common use cases to reusable hooks. *[source](https://www.wix.engineering/post/custom-react-hook-when-software-design-meets-react-hooks#:~:text=Custom%20hooks%20allow%20us%20to,use%20cases%20to%20reusable%20hooks.)*

### Using any list of custom hooks, research and name one that you think will be useful in your applications?

- I found a custom hook called `useLocalStorage` *[source](https://www.npmjs.com/package/@rehooks/local-storage)*.  This would be so helpful in my resty app because I forgot how to set localStorage. And I'm sure I'll forget it if I ever need to use it in another application. I just don't have much experience with setting local storage so any shortcut would be helpful!

### Describe how a hook that fetches API data might work

- You could use `useState` and `useEffect` to fetch API data. `useEffect` is usually used for these types of calls.

## Document the following vocab words

- **reducer:** a function that determines changes to an application's state. It uses the action it receives to determine this change. *[source](https://css-tricks.com/understanding-how-reducers-are-used-in-redux/#:~:text=A%20reducer%20is%20a%20function,so%20that%20they%20behave%20consistently.)*

## Preview

### Which 3 things had you heard about previously and now have better clarity on?

- Not familiar with Context, but hooks are becoming a little more clearer after all these different reading sources.

### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

- Context and hooks, and how they relate. Also more on the specific custom hooks like `useMemo` and `useReducer`

### What are you most excited about trying to implement or see how it works?

- Context, it sounds great to be able to pass data down without having to do props at every level.
