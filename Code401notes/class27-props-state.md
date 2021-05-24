# Class 27 Reading: Props and State

## Review, Research, and Discussion

### Does a deployed React application require a server?

- No when you do an `npx create-react-app`, it brings in all the necessary things for you to run the application

### Why do we prefer to test a React application at the behavior rather than the unit level?

- BDD tests are informed by the user acceptance criteria and should test the application from the user’s perspective to ensure that the user’s requirements are met.
- Unit tests are typically written by the implementing programmer, and test from the programmer's persepective.

### What does `npm run build` do?

- used in deployment - creates a build directory with a production build of your app *[source](https://create-react-app.dev/docs/deployment/)*

### Describe the actual composition/architecture of a React application

- Index.js is the "root" or ground of the the app. It is what you do the dom rendering.
- App.js is the main file usually and this is the Start component
- Other components are usually children to App.JS and App.js passes down props to those children components

## Document the following vocab words

- **BDD:** branch of Test Driven Development (TDD). BDD uses human-readable descriptions of software user requirements as the basis for software tests. *[source](https://medium.com/javascript-scene/behavior-driven-development-bdd-and-functional-testing-62084ad7f1f2)*
- **Acceptance Tests:** process of verifyng that a solution works for the user *[source](https://usersnap.com/blog/user-acceptance-testing-right/)*
- **mounting:** Mounting is the phase in which our React component mounts on the DOM (i.e., is created and inserted into the DOM).*[source](https://www.freecodecamp.org/news/how-to-understand-a-components-lifecycle-methods-in-reactjs-e1a609840630/)*
- **build:** the production version of your app during deployment

## Preview

### Which 3 things had you heard about previously and now have better clarity on?

- I'm familiar with setting state and handling events(usually with an onchange and then an onclick or onsubmit), I'm also familiar with using forms in react and the different components and how to pass props down to the additional components from App.

### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

- I'm not that familiar with React Testing. We didn't have to do much of that in the 301 course. If we did, the tests were already built for us.

### What are you most excited about trying to implement or see how it works?

- I'm also interested in learning more about the different roles and testing.
