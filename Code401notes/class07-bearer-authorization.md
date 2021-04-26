# Class 07 Reading: Bearer Authorization

## Review, Research, and Discussion

### Write the following steps in the correct order

- Register your application to get a client_id and client_secret
- Ask the client if they want to sign in via a third party
- Make a request to the access token endpoint
- Receive access token
- Redirect to a third party authentication endpoint
- Receive authorization code
- Make a request to a third-party API endpoint

### What can you do with an authorization code?

- The most common usage of authorization codes is those sent to a merchant from credit card issuers, to confirm that the customer's credit card has sufficient credit available to authorize the transaction. *[Source](https://www.investopedia.com/terms/a/authorization-code.asp#:~:text=An%20authorization%20code%20is%20an,into%20a%20security%2Dprotected%20space.)*

### What can you do with an access token?

- Access tokens are the thing that applications use to make API requests on behalf of a user. The access token represents the authorization of a specific application to access specific parts of a user’s data. *[Source](https://www.oauth.com/oauth2-servers/access-tokens/#:~:text=Access%20tokens%20are%20the%20thing,in%20transit%20and%20in%20storage.)*

### What's a benefit of using OAuth instead of your own basic authentication?

- End user knows they are giving their credentials to a trusted site
- Multi-factor authentication can be used
- End user can revoke access for the app at anytime
- User can allow the 3rd party app to access only certain information from her account
- Flow is entirely standardized

## Document the following vocab words

- **Client ID:** a public identifier for apps. *[source](https://www.oauth.com/oauth2-servers/client-registration/client-id-secret/)*
- **Client Secret:** a secret known only to the application and the authorization server. It must be sufficiently random to not be guessable, which means you should avoid using common UUID libraries which often take into account the timestamp or MAC address of the server generating it. *[source](https://www.oauth.com/oauth2-servers/client-registration/client-id-secret/)*
- **Authentication Endpoint:** is an authentication mechanism used to verify the identity of a network's external or remote connecting device. These endpoint devices include laptops, smartphones, tablets, and servers. *[source](https://www.iotone.com/term/end-point-authentication/t219)*
- **Access Token Endpoint:** is used by the client to obtain an access token by presenting its authorization grant or refresh token.  The token endpoint is used with every authorization grant except for the implicit grant type (since an access token is issued directly). *[source](https://tools.ietf.org/html/rfc6749#page-21)*
- **API Endpoint:** point of entry in a communication channel when two systems are interacting. It refers to touchpoints of the communication between an API and a server. *[source](https://rapidapi.com/blog/api-glossary/endpoint/#:~:text=In%20simple%20terms%2C%20an%20API,an%20API%20and%20a%20server.)*
- **Authorization Code:** an alphanumeric password that authorizes its user to purchase, sell or transfer items, or to enter information into a security-protected space. An authorization code is typically a sequence of letters, numbers, or a combination of both, that validates a person's identity, approves a transaction or provides access to a secured area. *[source](https://www.investopedia.com/terms/a/authorization-code.asp#:~:text=What%20Is%20an%20Authorization%20Code,into%20a%20security%2Dprotected%20space.)*
- **Access Token:** an object encapsulating the security identity of a process or thread.[1] A token is used to make security decisions and to store tamper-proof information about some system entity. *[source](https://en.wikipedia.org/wiki/Access_token#:~:text=An%20access%20token%20is%20an,information%20about%20some%20system%20entity.)*

## Preview

### Which 3 things had you heard about previously and now have better clarity on?

- I haven't heard of JWT before. I've used Auth0 in the past on 301 projects.

### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

- Anything about this topic of JWT because I don't believe I'm familiar with it at all

### What are you most excited about trying to implement or see how it works?

- Anything about JWT, I'm excited to see that in the code further.
