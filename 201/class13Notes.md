<sub>Think you might be in the wrong place? [Go home!](../README.md)</sub>



### Why would a developer use local storage for a web application?

* __Persistent Data Storage:__ Local storage provides a way to store data on the client side (in the user's web browser) that persists even after the user closes the browser or navigates away from the web page. This can be useful for saving user preferences, session information, or other data that needs to be retained between sessions.

* __Reduced Server Load:__ Storing data on the client side can reduce the need for frequent server requests to fetch the same data, improving the overall performance of a web application. This is particularly important for data that doesn't change frequently and can be cached on the client side.

* __Offline Capabilities:__ Local storage can be used to create offline-capable web applications. By storing essential data locally, the application can continue to function even when there is no internet connection.

### What information should not be stored in local storage?

* __Sensitive Information:__ Never store sensitive information such as passwords, credit card details, or personally identifiable information (PII) in local storage. This data should be handled on the server-side with appropriate security measures.

* __Large Amounts of Data:__ Local storage has a size limit (usually around 5-10 MB per domain), so it's not suitable for storing large datasets or files. Use other storage solutions like databases or cloud storage for such purposes.

* __Temporary Data:__ Local storage is designed for persistent data storage. It's not suitable for temporary data or data that needs to be frequently updated. For temporary data, use session storage or in-memory data structures.

### Local storage can store what type of data? How would you convert it to that type before storing?

* __Strings:__ Local storage primarily stores data as strings. You can store simple text values, JSON strings, or serialized data.

* __Numbers:__ You can store numeric values as strings in local storage and convert them back to numbers when retrieving them.

* __Booleans:__ Booleans can be stored as strings in local storage by converting them to "true" or "false" strings and parsing them back to booleans when retrieved.

To convert data to the appropriate type before storing it in local storage, you can use JavaScript's built-in methods like ``JSON.stringify()`` to convert objects or arrays to JSON strings. When retrieving the data, you can use ``JSON.parse()`` to convert the JSON string back into an object or array. For converting numeric and boolean values, you can use ``parseInt()`` and ``Boolean()`` functions, respectively, to ensure they are stored and retrieved as the correct data types.


<sub>Information gathered using ChatGPT</sub>