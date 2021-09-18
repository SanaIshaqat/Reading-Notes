# Code 301 Class 11 Reading notes:


## nosql vs sql

 ### Five differences between SQL and NoSQL databases:

SQL | NoSQL
------------ | -------------
SQL databases are primarily called as Relational Databases (RDBMS) | NoSQL database are primarily called as non-relational or distributed database
SQL databases are table based databases | NoSQL databases are document based, key-value pairs, graph databases or wide-column stores
SQL databases have predefined schema | NoSQL databases have dynamic schema for unstructured data
SQL databases are vertically scalable | NoSQL databases are horizontally scalable
SQL databases uses SQL ( structured query language ) for defining and manipulating the data, which is very powerful | NoSQL database, queries are focused on collection of documents. Sometimes it is also called as UnQL (Unstructured Query Language). The syntax of using UnQL varies from database to database

### What kind of data is a good fit for an SQL database? Give a real world example.
If your data is highly structured and associations among the program entities are clearly defined (for instance, if you are developing a point of sale system where you need to store customer orders and product records), conventional SQL based databases are the best fit.

### What kind of data is a good fit a NoSQL database? Give a real world example.
So, if your application requires high availability and scalability, a NoSQL Database built on BASE properties might be suitable. Choose NoSQL if you have or need: Semi-structured or Unstructured data / flexible schema. Limited pre-defined access paths and query patterns.

### Which type of database is best for hierarchical data storage?
NoSQL database fits better for the hierarchical data storage as it follows the key-value pair way of storing data similar to JSON data.
### Which type of database is best for scalability?
For scalability: In most typical situations, SQL databases are vertically scalable. You can manage increasing load by increasing the CPU, RAM, SSD, etc, on a single server. On the other hand, NoSQL databases are horizontally scalable. You can just add few more servers easily in your NoSQL database infrastructure to handle the large traffic.

### What does SQL stand for?
Structured Query Language
### What is a realational database?
A relational database is a type of database that stores and provides access to data points that are related to one another. 
### What type of structure does a relational database work with?
The relational model means that the logical data structures—the data tables, views, and indexes—are separate from the physical storage structures. This separation means that database administrators can manage physical data storage without affecting access to that data as a logical structure.
### What is a ‘schema’?
We define SQL Schema as a logical collection of database objects. A user owns that owns the schema is known as schema owner. It is a useful mechanism to segregate database objects for different applications, access rights, managing the security administration of databases.
### What is a NoSQL database?
NoSQL databases (aka "not only SQL") are non-tabular databases and store data differently than relational tables.
### How does it work?
NoSQL databases store data in documents rather than relational tables. Accordingly, we classify them as "not only SQL" and subdivide them by a variety of flexible data models. Types of NoSQL databases include pure document databases, key-value stores, wide-column databases, and graph databases.
### What is inside of a Mongo database?
Instead of using tables and rows as in the traditional relational databases, MongoDB makes use of collections and documents. Documents consist of key-value pairs which are the basic unit of data in MongoDB. Collections contain sets of documents and function which is the equivalent of relational database tables.
### Which is more flexible - SQL or MongoDB? and why.
While MongoDB is more flexible and ensures high and diverse data availability, a SQL Database operates with the ACID (Atomicity, Consistency, Isolation, and Durability) properties and ensures greater reliability of transactions.
### What is the disadvantage of a NoSQL database?
Disadvantages. NoSQL databases don't have the reliability functions which Relational Databases have (basically don't support ACID). This also means that NoSQL databases offer consistency in performance and scalability.


## Things I want to know more about
What is commonly more used SQl or NoSQL

#### Want To Know More ? 

[nosql vs sql](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool)