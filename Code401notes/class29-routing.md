# Class 29 Reading: Routing

## Review, Research, and Discussion

### Do child components have direct access to props/state from the parent?

- Only when the parent passes them down to the child component

### When a component "wraps" another component, how does the child component's output get rendered?

- It renders when the parent renders

### Can a component such as `<Content />`, which is a child also be used as a standalone component elsewhere in the application?

- Yes, this is what makes react so great, you can have reuse components in other places in your application. 

### What trick can a parent use to share all props with it's children?

- You can use `...`, which is the spread operator to pass all props to the child *[source](https://medium.com/coding-at-dawn/how-to-pass-all-props-to-a-child-component-in-react-bded9e38bb62)*

## Document the following vocab words

- **props.children:** used to display whatever you include between the opening and closing tags when invoking a component. *[source](https://codeburst.io/a-quick-intro-to-reacts-props-children-cb3d2fce4891)*
- **composition:** development pattern based on React's original component model where we build components from other components using explicit defined props or the implicit children prop. *[source](https://formidable.com/blog/2021/react-composition/)*

## Preview

### Which 3 things had you heard about previously and now have better clarity on?

- I have some experience using the browser router in 301 when we built out our react portfolio.

### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

- I'm not familiar with the react-if component. We did a lot of ternary statements in 301 react to decide which pages to render. Like with the router example.. if the user was not logged in, then take them to the login page. I'd like to see more info on that. Also the a more indepth on the testing library and aria roles. 

### What are you most excited about trying to implement or see how it works?

- More tricks around the browser router.
