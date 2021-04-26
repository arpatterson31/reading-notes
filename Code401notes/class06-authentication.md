# Class 06 Reading: Authentication

## Review, Research, and Discussion

### Explain what a "Singleton" is(in Computer Science terms)

- Also known as a unit set,[1] is a set with exactly one element. For example, the set {null } is a singleton containing the element null. The term is also used for a 1-tuple (a sequence with one member). *[Source](https://en.wikipedia.org/wiki/Singleton_(mathematics))*

### Explain how the Singleton pattern can be used with Node modules, specifically with classes

- Some examples include using a singleton as the source of config settings for a web app, on the client side for anything initiated with an API key (you usually don’t want to risk sending multiple analytics tracking calls, for example), and to store data in memory in a client-side web application (e.g. stores in Flux).
- Most of the time, going with an object literal is the most readable and concise option. However, there are times when you might want to exploit the benefits of going with a traditional class. For example, stores in Flux will all have a lot of the same base functionality. Leveraging traditional object-oriented inheritance is one way to get that repetitive functionality while keeping your code DRY.
- One benefit to the class route that might not be obvious is that, if this is your front-end code, and your back end is written in C# or Java, you can employ a lot of the same design patterns in your client-side application as you do on the back end, and increase your team’s efficiency (if you’re small and people are working full-stack). Sounds soft and hard to measure, but I’ve experienced it firsthand working on a C# application with a React front end, and the benefit is real.
- *[Source](https://www.sitepoint.com/javascript-design-patterns-singleton/)*

### If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?

- I would first try to figure out what I wanted my middleware to do and what would take to right the function for it. I would need the req, res, and next to construct/operate it.

## Document the following vocab words

- **Router Middleware:** Routing determines how the client requests are handled by the application endpoints. When you put your routers in separate file, you can use them by using middleware.
- **Dynamic Module Loading:**  mechanism by which a computer program can, at run time, load a library (or other binary) into memory, retrieve the addresses of functions and variables contained in the library, execute those functions or access those variables, and unload the library from memory. *[source](https://en.wikipedia.org/wiki/Dynamic_loading)*
- **Singleton Pattern:** In software engineering, the singleton pattern is a software design pattern that restricts the instantiation of a class to one "single" instance. This is useful when exactly one object is needed to coordinate actions across the system. The term comes from the mathematical concept of a singleton. *[Source](https://en.wikipedia.org/wiki/Singleton_pattern#:~:text=In%20software%20engineering%2C%20the%20singleton,mathematical%20concept%20of%20a%20singleton.)*
- **CRUD -> REST Method Matches:**
  - Create -> POST
  - Read -> GET
  - Update -> PUT
  - Delete -> DELETE
- **Mock Testing:** an approach to unit testing that lets you make assertions about how the code under test is interacting with other system modules. *[source](https://devopedia.org/mock-testing#:~:text=Mock%20testing%20is%20an%20approach,behaviour%20of%20the%20real%20ones.)*

## Preview

### Which 3 things had you heard about previously and now have better clarity on?

- In my 301 class we did a few projects using Auth0 so it is interesting in seeing other types of authentication in these readings/guidelines. 

### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

- A deeper dive into authentication, how to store passwords with the bcrypt package

### What are you most excited about trying to implement or see how it works?

- Anything about authentication! It makes websites seem a little more legit with that extra layer
