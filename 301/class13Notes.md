
<sub>Think you might be in the wrong place? [Go home!](../README.md)</sub>


### Which HTTP method would you use to update a record through an API?

To update a record through an __API__, the __HTTP__ method commonly used is __PUT__ or __PATCH__. The choice between PUT and PATCH depends on the semantics of the update operation.

* __PUT:__ Typically used to update a resource or create it if it doesn't exist. When you use PUT to update a resource, you generally send the full representation of the resource in the request.

* __PATCH:__ Used to apply partial modifications to a resource. It is often used when you want to update only specific fields of a resource, rather than sending the entire updated representation.

### Which REST methods require an ID parameter?

* __GET:__ Retrieve a resource.
* __PUT:__ Update a resource.
* __DELETE:__ Delete a resource.

### What’s the relationship between REST and CRUD?

__REST__ (Representational State Transfer) is an architectural style for designing networked applications, and __CRUD__ (Create, Read, Update, Delete) operations align with the standard HTTP methods in a RESTful API.

### If you had to describe the process of creating a RESTful API in 5 steps, what would they be?


* __Define Resources and Endpoints:__

    - Identify the entities/resources your API will expose.
    - Define unique URLs (endpoints) for each resource.
    
* __Use HTTP Methods for Operations:__

    - Map CRUD operations to appropriate HTTP methods.
    - POST for Create.
    - GET for Read.
    - PUT or PATCH for Update.
    - DELETE for Delete.

* __Design Data Formats:__

    - __Choose data formats for requests and responses__ (e.g., JSON or XML).
    - __Define clear and consistent data structures.__

* __Implement Server-Side Logic:__

  - Develop the server-side logic to handle requests.
  - Use frameworks or libraries that support routing, request handling, and database interactions.

 * __Handle Errors and Security:__

   * Implement error handling mechanisms, providing meaningful error responses.
   * Address security concerns (authentication, authorization, and secure communication).

   <sub>Information gathered using ChatGPT</sub>