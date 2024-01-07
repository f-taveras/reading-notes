<sub>Think you might be in the wrong place? [Go home!](../README.md)</sub>

### What is OAuth?

OAuth is an open standard for access delegation commonly used for secure communication between applications. It allows a user to grant a third-party application limited access to their resources without exposing their credentials (e.g., username and password). OAuth is widely used for enabling secure authentication and authorization in various scenarios, especially in the context of web and mobile applications.

### Give an example of what using OAuth would look like.

Let's consider an example where a user wants to log in to a third-party application (e.g., a mobile app) using their Google account. OAuth enables this process without the third-party application needing to store the user's Google credentials. The user is redirected to Google's authentication page, where they log in and authorize the third-party app to access specific information. Once authorized, the third-party app receives an access token to interact with the user's Google resources on their behalf.

### How does OAuth work? What are the steps that it takes to authenticate the user?

* __User Requests Access:__

    The user initiates a request to access a resource (e.g., logging in or granting permissions).

* __Authorization Server:__

    The third-party application sends the user to the authorization server (e.g., Google, Facebook) with a request for authorization.

* __User Authorizes Application:__

    The user authenticates themselves on the authorization server and grants permission to the third-party application.

* __Authorization Grant:__

    The authorization server generates an authorization grant (e.g., an authorization code) and sends it back to the third-party application.

* __Token Request:__

    The third-party application sends a token request to the authorization server, including the authorization grant.

* __Access Token Issued:__

    If the authorization grant is valid, the authorization server issues an access token to the third-party application.

* __Access Token Usage:__

    The third-party application uses the access token to access the user's resources on the resource server (e.g., Google API).

* __Resource Server Response:__

    The resource server responds with the requested data if the access token is valid.

### What is OpenID?

OpenID is often used in conjunction with OAuth to provide user authentication. While OAuth deals with authorization, OpenID focuses on authentication. OpenID allows users to use a single set of credentials (OpenID) to access multiple applications or websites. The OpenID Connect (OIDC) protocol is built on top of OAuth 2.0 and adds authentication capabilities.

<sub>Information gathered using ChatGPT</sub>