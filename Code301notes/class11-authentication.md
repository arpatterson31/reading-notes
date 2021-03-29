# Readings: Authentication

## Article - What is OAuth?

- **OAUTH** allows websites and services to share assets among users
  - Open-standard authorization protocol or framework

### OAUTH Examples

- Logging into a website and using another website's/service's logon.
  - Like using your Google or GitHub account to login to a site
- User sending cloud-stored files to another user via email
  - Google Gmail or Microsoft OneDrive
- End user using a 3rd party printing service to print pictures files stored on an unrelated web server

- OAuth almost always represents 2 unrelated sites or services trying to accomplish something on behalf of users or their software

- OAuth is about authorization, not authentication

### How OAuth works

1. website connects to the 2nd website on behalf of the user, providing user's verified identity
2. 2nd site generates a one-time token and a one-time secret unique to the parties involved
3. 1st site gives this token and secret to the initiating user's clients software
4. Client's software presents the token to their authorization provider
5. User is given a access token (no longer a request token)
6. Tokens are exchanged and then the 2nd website lets the first website in on behalf of the user

- **OpenID** is similiar except it is for humans logging into machines, OAuth is for machines logging into machines on behalf of humans

- **SAML** (Security Assertion Markup Language) allows one computer to perform both authentication and authorization on behalf of the comptuers (My previous employer used this with our SSO integration - Okta)

## Article - Authentication and Authorization Flows

### Authentication vs Authorization

|**Authentication** | **Authorization** |
|-------------------|-----------------------|
| Determines whether users are who they say they are | Determines what users can/cannot access |
| done before authorization | done after successful authentication |
| makes the user validate credentials like security questions or facial recognition | verifies whether access is allowed through policies or rules |
| transmits info through an ID token | transmits info through access token |
|governed by OpenID Connect | governed by OAuth 2.0 |

### Authorization Code Flow

#### Authorization Code Flow - exchanges an authorization code for a token

![Authorization Code Flow](https://images.ctfassets.net/cdy7uua7fh8z/2nbNztohyR7uMcZmnUt0VU/2c017d2a2a2cdd80f097554d33ff72dd/auth-sequence-auth-code.png)

- [Adding Login using Authorization Code Flow](https://auth0.com/docs/flows/add-login-auth-code-flow)
- [Call API using Authorization Code Flow](https://auth0.com/docs/flows/call-your-api-using-the-authorization-code-flow)

#### Authorization Code Flow w/ Proof Key for Code Exchange - used when mobile and native applications require additional security

![PKCE](https://images.ctfassets.net/cdy7uua7fh8z/3pstjSYx3YNSiJQnwKZvm5/33c941faf2e0c434a9ab1f0f3a06e13a/auth-sequence-auth-code-pkce.png)

- [Adding Login with PKCE](https://auth0.com/docs/flows/add-login-using-the-authorization-code-flow-with-pkce)
- [Call API with PKCE](https://auth0.com/docs/flows/call-your-api-using-the-authorization-code-flow-with-pkce)

## Auth0 React SDK

- Installation

`npm install @auth0/auth0-react`

- Getting Started - wrap your application in a single `Auth0Provider` component. This provides React Context to components that are placed inside your application

````javascript
 import React from 'react';
    import ReactDOM from 'react-dom';
    import { Auth0Provider } from '@auth0/auth0-react';
    import App from './App';
    ReactDOM.render(
      <Auth0Provider
        domain="YOUR_DOMAIN"
        clientId="YOUR_CLIENT_ID"
        redirectUri={window.location.origin}
    >
      <App />
    </Auth0Provider>,
    document.getElementById('app')
 );
 ````

- isLoading and error - wait for SDK to initialize and handle any errors using `isLoading` and `error` states

````javascript
import React from 'react';
import { useAuth0 } from '@auth0/auth0-react';
function Wrapper({ children }) {
  const {
    isLoading,
    error,
  } = useAuth0();
  if (isLoading) {
    return <div>Loading...</div>;
  }
  if (error) {
    return <div>Oops... {error.message}</div>;
  }
  return <>{children}</>;
}
export default Wrapper;
````

- Login - use `loginWithRedirect` or `loginWithPopup`

````javascript
import React from 'react';
import { useAuth0 } from '@auth0/auth0-react';

function LoginButton() {
  const {
    isAuthenticated,
    loginWithRedirect,
  } = useAuth0();

  return !isAuthenticated && (
    <button onClick={loginWithRedirect}>Log in</button>
  );
}

export default LoginButton;
````

- Logout - use `logout`... make sure `returnTo` is specified

````javascript
import React from 'react';
import { useAuth0 } from '@auth0/auth0-react';

function LogoutButton() {
  const {
    isAuthenticated,
    logout,
  } = useAuth0();

  return isAuthenticated && (
    <button onClick={() => {
      logout({ returnTo: window.location.origin });
    }}>Log out</button>
  );
}

export default LogoutButton;
````

- Class Component

````javascript
import React, { Component } from 'react';
import { withAuth0 } from '@auth0/auth0-react';

class Profile extends Component {
  render() {
    const { user } = this.props.auth0;
    return <div>Hello {user.name}</div>;
  }
}

export default withAuth0(Profile);
````

- API Calls - specify `audience` and `scope` of your access token either in `Auth0Provider` or `getAccessTokenSilently`. Pass it in the `Authorization` header of your request

````javascript
import React, { useEffect, useState } from 'react';
import { useAuth0 } from '@auth0/auth0-react';

const Posts = () => {
  const { getAccessTokenSilently } = useAuth0();
  const [posts, setPosts] = useState(null);

  useEffect(() => {
    (async () => {
      try {
        const token = await getAccessTokenSilently({
          audience: 'https://api.example.com/',
          scope: 'read:posts',
        });
        const response = await fetch('https://api.example.com/posts', {
          headers: {
            Authorization: `Bearer ${token}`,
          },
        });
        setPosts(await response.json());
      } catch (e) {
        console.error(e);
      }
    })();
  }, [getAccessTokenSilently]);

  if (!posts) {
    return <div>Loading...</div>;
  }

  return (
    <ul>
      {posts.map((post, index) => {
        return <li key={index}>{post}</li>;
      })}
    </ul>
  );
};

export default Posts;
````
