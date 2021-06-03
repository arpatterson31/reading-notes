# Class 34 Reading: `<Login />` and `<Auth />`

## Review, Research, and Discussion

### Why is the Context API useful?

- It is a way for a React app to effectively produce global variables that can be passed around. This is the alternative to "prop drilling" or moving props from grandparent to child to parent, and so on. Context is also touted as an easier, lighter approach to state management using Redux. *[source](https://www.loginradius.com/blog/async/react-context-api/#:~:text=The%20React%20Context%20API%20is,to%20state%20management%20using%20Redux.)*

### Can a component outside of a provider get its context?

- The most common way to access Context from a class component is via the static contextType . If you need the value from Context outside of render , or in a lifecycle method, you'll use it this way. The traditional way to retrieve Context values was by wrapping the child component in the Consumer *[source](https://www.taniarascia.com/using-context-api-in-react/)*

### What are some common use cases for using the Context API?

- Themes: setting UX themes; Multilingual applications; Authorization: setting user role and info *[source](https://blog.bitsrc.io/why-you-should-consider-the-new-context-api-in-react-a-deep-dive-d588b66c57b5)*

### Describe "Context Hell"?

- "Nasty code" you get when using the Context API where there are multiple Context.Providers being passed as children of each other *[source](https://dev.to/alfredosalzillo/the-react-context-hell-7p4)*

## Document the following vocab words

- **global state:** data that doesn't have to be passed down as props manually at every level
- **global context:** Context that is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language. *[source](https://reactjs.org/docs/context.html)*
- **provider:** component that allows consuming components to subscribe to context changes. *[source](https://reactjs.org/docs/context.html#contextprovider)*
- **consumer:** A React component that subscribes to context changes. *[source](https://reactjs.org/docs/context.html#contextconsumer)*

## Preview

### Which 3 things had you heard about previously and now have better clarity on?

- Role Based access control, I'm familiar with cookies but not using them in React

### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

- Looking to dive more into the auth on React. We used Auth0 in 301. Also looking forward to learning more about using cookies. 

### What are you most excited about trying to implement or see how it works?

- Context API, Cookies
