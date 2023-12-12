<sub>Think you might be in the wrong place? [Go home!](../README.md)</sub>



In your own words, describe what each group of status code represents:

* __100’s__ = Indicates the request has been received and understood.
* __200’s__ = __(Successful)__ Indicates successful request processing.
* __300’s__ = __(Redirection)__ Indicates further action or redirection is needed.
* __400’s__ = __(Client Error)__ Indicates client-side errors or invalid requests.
* __500’s__ = __(Server Error)__ Indicates server-side errors.
* __What is a status code 202?__ 

    __Accepted__ Indicates the request was accepted but not yet processed.

* __What is a status code 308?__

    __Permanent Redirect:__ Indicates the requested resource has been permanently moved.

* What code would you use if an update didn’t return data to a client?

    __204__ (__No Content__) Indicates a successful request with no content returned.

* What code would you use if a resource used to exist but no longer does?

    __410__ (__Gone__) Indicates the requested resource is no longer available.

* What is the ‘Forbidden’ status code?

__403__ __(Forbidden)__ Indicates the client lacks necessary permissions.


### Why do we need to pull our MongoDB database string out of our server and put it into our .env?

Storing sensitive information, such as database connection strings, in the __.env__ file adds a layer of security. It keeps sensitive data separate from the codebase and allows developers to use different configurations for development, testing, and production environments without modifying the code.

### What is middleware?

Middleware is software that acts as a bridge between an application and its database, server, or other components. In the context of web development, middleware functions have access to the request and response objects, and they can perform tasks such as modifying the request, response, or executing additional code before reaching the final route handler.

### What does app.use(express.json()) do?

This middleware in __Express.js__ is used to parse incoming __JSON__ requests. It enables the server to understand and work with __JSON__ data sent in the request body, making it accessible through __req.body__ in route handlers.

### What does the /:id mean in a route?

It represents a route parameter in Express.js. The value specified in the URL at the position of :id is captured and made available as req.params.id in the route handler. This allows dynamic handling of requests with varying IDs.

### What is the difference between PUT and PATCH?

* __PUT:__ Typically used to update or replace an entire resource. The request payload should contain the complete updated resource.

* __PATCH:__ Used to apply partial modifications to a resource. The request payload contains only the changes, allowing for more granular updates.

### How do you make a default value in a schema?

In a __MongoDB__ schema, you can set a default value for a field using the default property. For example:

```
const UserSchema = new Schema({
  name: {
    type: String,
    default: 'John Doe',
  },
});
```
### What does a 500 error status code mean?

A __500__ Internal Server Error status code indicates that the server encountered an unexpected condition that prevented it from fulfilling the request. It is a generic error message when the server encounters an error not specifically handled by the application.

### What is the difference between a status 200 and a status 201?

* __Status 200 OK:__ Indicates that the request was successful.

* __Status 201 Created:__ Indicates that the request was successful, and a new resource was created as a result. It is often used in response to successful POST requests to signify the creation of a new resource.

<sub>Information gathered using ChatGPT</sub>