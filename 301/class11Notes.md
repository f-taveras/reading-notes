<sub>Think you might be in the wrong place? [Go home!](../README.md)</sub>

| SQL      | NoSQL |
| ----------- | ----------- |
| __DataStructure__      | SQL databases are table-based and follow a rigid, structured schema. Each row in a table represents a record, and columns define the data types.
| Scalability   | SQL databases are typically scaled vertically by increasing the horsepower (CPU, RAM, SSD) on a single server.
| ACID Properties   | SQL databases follow ACID properties (Atomicity, Consistency, Isolation, Durability) to ensure the reliability of transactions.
|Query Language   | SQL databases use SQL (Structured Query Language) for defining and manipulating the data.
| Example Databases | Examples of SQL databases include MySQL, PostgreSQL, and Oracle.
   |



### What kind of data is a good fit for an SQL database?

* __Data with Well-Defined Structure:__ SQL databases are suitable for data with a well-defined and consistent structure. If your data fits neatly into tables with predefined relationships, SQL is a good choice.

* __Online Retail System:__ A relational database can be used to store information about customers, orders, products, and inventory in a structured manner. Each table (e.g., Customers, Orders, Products) has predefined columns and relationships.



### What kind of data is a good fit a NoSQL database?

* __Unstructured or Semi-Structured Data:__ NoSQL databases are suitable for data with a flexible or changing structure. If your data is document-oriented, hierarchical, or doesn't fit neatly into tables, NoSQL can be a good fit.
Real-World Example:

* __Content Management System (CMS):__ NoSQL databases like MongoDB are suitable for storing content in a CMS. Content can vary in structure and include documents, images, metadata, and user-generated content.



### Which type of database is best for hierarchical data storage?

* __NoSQL Database (Document Store):__ NoSQL databases, especially document stores, are well-suited for hierarchical data storage. The nested and nested-array structures in documents align well with hierarchical data.

### Which type of database is best for scalability?

* __NoSQL Database (Distributed):__ NoSQL databases, designed for horizontal scalability, are well-suited for handling large amounts of data and traffic. Adding more servers to a NoSQL database helps achieve scalability.



### What does SQL stand for?

> SQL stands for Structured Query Language.

### What is a relational database?

A relational database is a type of database that uses a structure that allows us to identify and access data in relation to another piece of data in the database. It's based on the relational model of data, where data is stored in tables and relationships between the tables are established using keys.

### What type of structure does a relational database work with?

A relational database works with a tabular structure, organizing data into tables with rows and columns. Tables have predefined relationships with one another through keys (primary and foreign keys).

### What is a ‘schema’?

A _schema_ in the context of a relational database is a collection of database objects, including tables, views, indexes, and constraints. It defines the structure of the database, specifying how data is organized and related.

### What is a NoSQL database?

__NoSQL__ (Not Only SQL) databases are a type of database that provides a mechanism for the storage and retrieval of data that is modeled in a way other than the tabular relations used in relational databases.

### How does it work?

__NoSQL__ databases work with various data models, including document, key-value, column-family, and graph formats. They are designed to be more flexible, scalable, and capable of handling unstructured or semi-structured data.

### What is inside of a MongoDB database?

A __MongoDB__ database consists of collections, which are akin to tables in relational databases, and documents, which are similar to rows but can have varying structures. MongoDB uses BSON (Binary JSON) format to store data.

### Which is more flexible - SQL or MongoDB? and why.

__MongoDB__ is generally considered more flexible than SQL databases. MongoDB's document-oriented structure allows for dynamic schemas, meaning each document in a collection can have a different structure. This flexibility is useful for handling evolving or unstructured data.
### What is the disadvantage of a NoSQL database?

One disadvantage of NoSQL databases is the lack of standardized querying language (unlike SQL in relational databases). Each NoSQL database may have its query language or API, making it less uniform for developers who work with different databases. Additionally, some NoSQL databases may lack the transactional consistency provided by relational databases, which can be a drawback in certain scenarios.

<sub>Information gathered using ChatGPT</sub>