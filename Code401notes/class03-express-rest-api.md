# Class 03 Reading: Express REST API

## Review, Research, and Discussion

### Name 3 real world use cases where you'd want to change the request with custom middleware

- **Translator** - uses a data conversion library and translates requests to a format that the receiving service can understand *[Source](https://www.freecodecamp.org/news/what-is-middleware-with-example-use-cases/)*
- **Duplicating Data** - can store duplicate data in search server so it can search them instead of requesting from product and user servers *[Source](https://www.freecodecamp.org/news/what-is-middleware-with-example-use-cases/)*
- **Auth** - can verify user information once authenticated with login information

### True or false: the route handler is middleware?

### In what ways can a middleware function end the process and send data to the browser?

### At what point in the request lifecycle can you “inject” middleware?

### What can cause express to error with “Request headers sent twice, cannot start a second response”

## Document the following Vocab Terms

- **Middleware:** Express middleware are functions that execute during the lifecycle of a request to the Express server
- **Request Object:** represents the HTTP request and has properties for the request query string, parameters, body, HTTP headers, and so on *[Source](http://expressjs.com/en/4x/api.html#req)*
- **Response Object:** represents the HTTP response that an Express app sends when it gets an HTTP request. *[Source](http://expressjs.com/en/4x/api.html#res)*
- **Application Middleware:**  middleware bound to the app object by using the `app.use()` and `app.METHOD()` functions - *[Source](https://expressjs.com/en/guide/using-middleware.html#middleware.application)*
- **Routing Middleware:**  middleware bound to an instance of `express.Router()` *[Source](https://expressjs.com/en/guide/using-middleware.html#middleware.router)*
- **Test Driven Development:** process of writing tests first then your code
- **Behavioral Testing:** a testing of the external behaviour of the program, also known as black box testing. It is usually a functional testing. *[Source](https://www.tutorialspoint.com/software_testing_dictionary/behaviour_testing.htm#:~:text=Behavioural%20Testing%20is%20a%20testing,is%20usually%20a%20functional%20testing.)*
