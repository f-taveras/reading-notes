<sub>Think you might be in the wrong place? [Go home!](../README.md)</sub>

# What is the primary purpose of JSON Web Tokens (JWTs) and how do they work in terms of encoding and decoding data?

__JSON Web Tokens (JWTs)__ are an open, industry standard method (RFC 7519) for representing claims securely between two parties. The primary purpose of JWTs is to securely transmit information between parties as a compact, URL-safe means. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.

JWTs consist of three parts separated by dots __(.)__:

* __Header:__ The header typically consists of two parts: the type of the token, which is __JWT__, and the signing algorithm being used, such as __HMAC SHA256__ or __RSA__.
* __Payload:__ The payload contains the claims. Claims are statements about an entity (typically, the user) and additional data. There are three types of claims: registered, public, and private claims.
* __Signature:__ To create the signature part, you have to take the encoded header, the encoded payload, a secret, the algorithm specified in the header, and sign that.

The JWT is then a combination of these three parts, encoded in Base64Url, creating a compact and URL-safe token.

__Decoding__ a JWT does not require a secret; it can be done by simply decoding the Base64Url encoded parts. However, to verify the signature of a JWT, the secret or key used to sign the token is required. This ensures that the sender of the JWT is who it claims to be and that the message hasn't been altered.

# How does JWT Authentication integrate with Django REST Framework to secure API endpoints, and what are the key components involved in this process?

__JWT Authentication__ integrates with the Django REST Framework (DRF) to secure API endpoints by ensuring that only authenticated users can access certain resources. The key components involved in this process include:

* __JWT Authentication Class:__ A custom authentication class that extends Django REST Framework's authentication classes. This class processes the JWT from the __Authorization__ header of incoming requests to authenticate the user.
* __Token Generation and Validation__: When a user logs in, a JWT is generated using the user's credentials and returned to the user. This token must be included in the __Authorization__ header of subsequent requests. The JWT authentication class validates this token by verifying its signature and checking its expiration.
* __User Model and Authentication Backend:__ The user's identity is determined based on the payload of the JWT, which typically includes user-related claims like user ID. DRF uses this information to set the user in the request context, allowing views to access the authenticated user.
* __Secure API Endpoints:__ By applying the JWT authentication class to API views or globally, only requests with valid JWTs can access those endpoints, thus securing them against unauthorized access.

# Why is Django’s built-in runserver not suitable for production environments, and what are some alternative server options that should be considered for deploying a Django application?

Django’s built-in development server (`runserver`) is not suitable for production for several reasons:

* __Performance:__ It is single-threaded and not designed to handle high volumes of traffic efficiently.
* __Security:__ It lacks security features necessary to protect against attacks and vulnerabilities in a production environment.
* __Reliability:__ It doesn’t include features needed for a stable environment, such as handling of static files and media in an efficient manner.

For deploying a Django application in a production environment, it's recommended to use a more robust WSGI (Web Server Gateway Interface) server. __Some of the popular options include:__

* __Gunicorn:__ A pre-forked, partly asynchronous server that is easy to configure and use.
* __uWSGI:__ A versatile and highly configurable server that implements WSGI, uwsgi, and http protocols.
* __Daphne:__ An HTTP, HTTP2, and WebSocket protocol server for ASGI and 
ASGI-HTTP, suitable for Django channels.

These servers are typically used behind a full-featured web server like Nginx or Apache that can serve static files, handle HTTPS, and proxy requests to the WSGI server. This setup ensures efficiency, security, and scalability for Django applications in production.

<sub>Information modeled using ChatGPT</sub>
