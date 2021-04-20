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
