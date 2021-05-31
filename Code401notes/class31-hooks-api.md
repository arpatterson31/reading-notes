# Class 31 Reading: Hooks API

## Review, Research, and Discussion

### Why do we not need more .html pages in a multi-page React app?

- React is considered a "single page application" so when we build "multi-pages", what is happening, is that a component renders specificially for that route.

### If we wanted a component to show up on every page, were would we put it and why?

- We would start by putting everything in a `<BrowserRouter />` becasue that wraps the whole page. But if we want to a specific component to show up on every page then we would want it outside of a `<Route />` so that will render with whatever route a user visits.

### What does props.children contain?

- This contains any element you include between opening and closing tags when invoking a component. *[source](https://stackoverflow.com/questions/49706823/what-is-this-props-children-and-when-you-should-use-it#:~:text=of%20what%20this.-,props.,used%20to%20create%20a%20component.)*

## Document the following vocab words

- **composition:** development pattern based on React's original component model where we build components from other components using explicit defined props or the implicit children prop. *[source](https://formidable.com/blog/2021/react-composition/)*
- **children/child components:** a react component that is nested within a parent component
- **hash routing:** application endpoint controlled by one single back-end action and multiple hashtags managed by Javascript that define the SPA routes. *[source](https://itnext.io/why-using-hash-based-urls-in-your-react-spa-will-save-you-more-time-than-you-think-a21e2c560879)*
- **link routing:** Provides declarative, accessible navigation around your application. *[source](https://reactrouter.com/web/api/Link)*

## Preview

### Which 3 things had you heard about previously and now have better clarity on?

- I dont have any experience in using Hooks in React. This was something we were told that we couldn't use in 301.

### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

- For sure the hooks. Also I'd like to get more information on the routing because I struggled a little bit with using the If, Then, Else, when it came to routing my page. 

### What are you most excited about trying to implement or see how it works?

- The hooks! I was told that these are a godsend to react!
