# Readings: CRUD

## MDN Web Docs - Sending Form Data

### What happens when a user submits a form?

### Client/Server Architecture

- Web uses a client/server architecture
  - client or web browser sends a request to a server using the HTTP protocol
  - Server answers the request using the same protocol

![Client Server Architecture](https://developer.mozilla.org/en-US/docs/Learn/Forms/Sending_and_retrieving_form_data/client-server.png)

### Client Side

- `<form>` element defines how the data will be sent
- 2 most important attributes are `action` and `method`

#### Action Attribute

- `action` defines where the data gets sent
  - must be a valid relative path or absolute URL
  - if no `action` is provided, data will be sent to the URL of the page containing the form

#### Examples

- `<form action="https://example.com>`
- `<form action="/somewhere_else>`

#### Method Attribute

- `method` defines how the data is sent
  - `GET method` - used by browser to ask the server to send back a given resource
  - `POST method` - used by browser to talk to the server when asking for a response that takes into accont the data provided

### Server Side

- No matter which method used, the server receives a string that will be parsed in order to get the data as a list of key/value pairs

### Security

- When you send data to a server, you need to consider security
- HTML forms are the most common server attack vectors
