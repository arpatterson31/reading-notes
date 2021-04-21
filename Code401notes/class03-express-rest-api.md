# Class 03 Reading: Express REST API

## Review, Research, and Discussion

### Name 3 real world use cases where you'd want to change the request with custom middleware

- **Translator** - uses a data conversion library and translates requests to a format that the receiving service can understand *[Source](https://www.freecodecamp.org/news/what-is-middleware-with-example-use-cases/)*
- **Duplicating Data** - can store duplicate data in search server so it can search them instead of requesting from product and user servers *[Source](https://www.freecodecamp.org/news/what-is-middleware-with-example-use-cases/)*
- **Auth** - can verify user information once authenticated with login information

### True or false: the route handler is middleware?

- **True** in some situations. When a routing method passes a function that has `req`, `res`, and `next`, then it is both a middleware function and a handler function *[source](https://stackoverflow.com/questions/58925276/what-is-the-difference-between-a-route-handler-and-middleware-function-in-expres#:~:text=They%20are%20not%20middleware%20functions,they%20are%20only%20handler%20functions.)*

### In what ways can a middleware function end the process and send data to the browser?

- If the middleware does not call `next()` or it can call `res.end` *[source](https://stackoverflow.com/questions/33648905/after-sending-response-how-to-end-the-current-request-processing-in-node-expres)*

### At what point in the request lifecycle can you “inject” middleware?

- Middleware is a function which is called before the route handler. Middleware functions have access to the request and response objects, and the `next()` middleware function in the application’s request-response cycle. The next middleware function is commonly denoted by a variable named next. *[source](https://docs.nestjs.com/middleware)*

### What can cause express to error with “Request headers sent twice, cannot start a second response”

- The server tries to send more than one response to a client. What this means is that for a given client request the server previously sent a response (either a success response with the resource requested or error response for a bad request) back to the client and now is unexpectedly trying to send another response *[Source](https://www.codementor.io/@oparaprosper79/understanding-node-error-err_http_headers_sent-117mpk82z8)*

## Document the following Vocab Terms

- **Middleware:** Express middleware are functions that execute during the lifecycle of a request to the Express server
- **Request Object:** represents the HTTP request and has properties for the request query string, parameters, body, HTTP headers, and so on *[Source](http://expressjs.com/en/4x/api.html#req)*
- **Response Object:** represents the HTTP response that an Express app sends when it gets an HTTP request. *[Source](http://expressjs.com/en/4x/api.html#res)*
- **Application Middleware:**  middleware bound to the app object by using the `app.use()` and `app.METHOD()` functions - *[Source](https://expressjs.com/en/guide/using-middleware.html#middleware.application)*
- **Routing Middleware:**  middleware bound to an instance of `express.Router()` *[Source](https://expressjs.com/en/guide/using-middleware.html#middleware.router)*
- **Test Driven Development:** process of writing tests first then your code
- **Behavioral Testing:** a testing of the external behaviour of the program, also known as black box testing. It is usually a functional testing. *[Source](https://www.tutorialspoint.com/software_testing_dictionary/behaviour_testing.htm#:~:text=Behavioural%20Testing%20is%20a%20testing,is%20usually%20a%20functional%20testing.)*

## Preview

### Which 3 things had you heard about previously and now have better clarity on?

- Request Object, and Response Object..also did a lot of work with the ES6 Classes in 301

### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

- Still would like more clarity on middleware and the different of use cases there. Was pretty comfortable with routing from the 301 projects, but would like more clarity on adding all the extra params and middleware.

### What are you most excited about trying to implement or see how it works?

- More of the TDD, I'm starting to understand more about how to write the tests but not sure on the why
