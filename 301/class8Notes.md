<sub>Think you might be in the wrong place? [Go home!](../README.md)</sub>

### What does REST stand for?

__REST__ stands for Representational State Transfer.

### REST APIs are designed around a ____.

stateless client-server architecture.

### What is an identifier of a resource? Give an example.

An identifier of a resource is typically a URI _(Uniform Resource Identifier)_. Example: https://api.example.com/users/123

### What are the most common HTTP verbs?

* __GET:__ Retrieve a resource.
* __POST:__ Create a new resource.
* __PUT:__ Update an existing resource.
* __DELETE:__ Delete a resource.

### What should the URIs be based on?

URIs (Uniform Resource Identifiers) should be based on the resources they identify.

### Give an example of a good URI.

Example of a good URI: https://api.example.com/products/42

### What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?

Having a _'chatty'_ web API means that it requires a high number of requests to perform a single operation. This is generally considered a bad thing because it can result in increased network latency and reduced performance.

### What status code does a successful GET request return?

A successful GET request returns a status code of 200 OK.

### What status code does an unsuccessful GET request return?

An unsuccessful GET request can return various status codes, but a common one is __404 Not Found__ if the requested resource is not available.

### What status code does a successful POST request return?

A successful POST request returns a status code of __201__ Created if a new resource is successfully created.

### What status code does a successful DELETE request return?

A successful __DELETE__ request returns a status code of __204__ No Content to indicate that the resource has been successfully deleted.
<sub>Information gathered using ChatGPT</sub>