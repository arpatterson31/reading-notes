# Class 02 Reading: Express

## Review, Research, and Discussion

**What is the difference between `PUT` and `PATCH`?**

- `PUT` and `PATCH` both update in CRUD functionality, but they do it differently. `PUT` is a method of modifying resource where the client sends data that updates the entire resource. `PATCH` applies a partial update to the resource

*Source: [Rapid API](https://rapidapi.com/blog/put-vs-patch/)*

**Provide links to 3 services or tools that allow you to 'mock' an API for development like `json-server`**

- [Mirage js](https://www.valentinog.com/blog/fake/#mirage-js)

````javascript
npm i miragejs --save-dev
````

- [Jest](https://jestjs.io/)

````javascript
npm i jest --save-dev
````

- [Postman](https://www.postman.com/features/mock-api/)
  - [Mock API docs](https://learning.postman.com/docs/designing-and-developing-your-api/mocking-data/setting-up-mock/)

**Compare and constrast Swagger and APIDoc.js**

- Both are documentation tools
- **apiDocsjs:** Inline Documentation for RESTful web APIs. It creates a documentation from API annotations in your source code. It includes a default template which uses handlebars, Bootstrap, RequireJS and jQuery for the output of the generated apidata.js and apiproject.js as a html-page
- **Swagger Inspector:** Test and Document Your APIs With Ease. It is a free cloud-based API testing and documentation tool to simplify the validation of any API and generate its corresponding OpenAPI documentation.
- *Source [Stackshare](https://stackshare.io/stackups/apidocjs-vs-swagger-inspector)*

**Which HTTP Status codes should be sent with each type of (un)successful API Call?**

- 1xx: Informational - Communicates transfer protocol-level info
- 2xx: Success - Indicates that the client's request was accepted successfully
- 3xx: Redirection - Indicates that the client must take some additional action in order to complete their request
- 4xx: Client Error - This category of error status codes points the finger at clients
- 5xx: Server Error - The server takes responsibility for these error status codes
- *Source: [Restfulapi.net](https://restfulapi.net/http-status-codes/)*

**Compare and Contrast SOAP and ReST**

- **SOAP:** Simple Object Access Protocol - designed to ensure programs built on different platforms and with different languages can exchange data in an easy manner
  - protocol
  - only works with XML formats
  - can not make use of REST

- **ReST:** Representational State Transfer - designed for working with components like media, files, or objects
  - architectural pattern
  - works with plain text, HTML, XML, and JSON
  - can make use of SOAP

### Document the following Vocab Terms

- **Web Server:** computer software that accepts requests via HTTP or HTTPS *[Source](https://en.wikipedia.org/wiki/Web_server)*
- **Express:** back end web application framework for Node.js *[Source](https://en.wikipedia.org/wiki/Express.js)*
- **Routing:** selecting a path for requests that are routed to the code that handles them
- **WRRC:** Web Request Response Cycle - traces how a user's request flows through the app *[Source](https://www.codecademy.com/articles/request-response-cycle-static)*

### Preview

**Which 3 things had you heard about previously and now have better clarity on?**

- Express - this is still very fresh in my mind coming out of 301 a week ago
- route handlers I have used in the past labs
- I have also used NPM in the past 301 labs - especially when working with react

**Which 3 things are you hoping to learn more about in the upcoming lecture/demo?**

- TDD for sure, this is a new concept for me
- all the additional parameters in the route handlers like next
- more realword examples for middleware!

**What are you most excited about trying to implement or see how it works?**

- Building out the tests seems exciting now. We did a lot of debugging and had a big part of that in our 301 final exam. As much as that was really intimidating, I'm excited to learn how to continue to write my own tests.
