# Reading Notes

## MongoDB and Mongoose

Fill in the chart below with five differences between SQL and NoSQL databases:

| SQL | NoSql |
|:------------:|:--------------:|
| Relational Databases (RDBMS)     |  Non-relational or distributed database.         |
| table based databases  | Document based, key-value pairs, graph databases or wide-column stores      |
| predefined schema   | Cdynamic schema for unstructured data         |
| vertically scalable     | horizontally scalable      |
| structured query language       | Queries are focused on collection of documents.        |
| MySql, Oracle, Sqlite, Postgres and MS-SQL      | MongoDB, BigTable, Redis, RavenDb, Cassandra, Hbase, Neo4j and CouchDb         |

What kind of data is a good fit for an SQL database?

Product information, including product IDs, names, descriptions, prices, and current stock levels..

Give a real world example.

Walmart is a large company and uses doing alot of transacton.

What kind of data is a good fit a NoSQL database?

key-value stores are suitable for scenarios where data is represented as simple key-value pairs.

Give a real world example.

online retail and e-commerce applications. you have a vast amount of data to manage, including product information, customer profiles, orders, and user activity.

Which type of database is best for hierarchical data storage?

 NoSQL database

Which type of database is best for scalability?

MySQL

What does SQL stand for?

Structured Query Language

What is a relational database?

Is a type of database that uses a relational model to organize and store data.

What type of structure does a relational database work with?

* Tables

* Rows (Tuples):

* Columns (Attributes):

* Keys

* Relationships

What is a ‘schema’?

refers to the logical structure or blueprint that defines the organization of data within a database. It defines the layout of tables, the relationships between them, and the constraints applied to the data.

What is a NoSQL database?

A NoSQL database is a type of database management system (DBMS) that provides a mechanism for storing and retrieving data that is modeled in ways other than the traditional tabular relations used in relational databases. The term "NoSQL" stands for "Not Only SQL," indicating that these databases may support query languages other than SQL, and they are not strictly adherent to the relational model.

How does it work?

The way a NoSQL database works depends on the specific type of NoSQL database, as there are various models, including document stores, key-value stores, wide-column stores, and graph databases.

What is inside of a MongoDB database?

data is organized into collections, each of which contains documents. A document is a set of key-value pairs, where each key represents a field and its associated value. Documents, resembling JSON-like structures, serve as the fundamental unit of data in MongoDB and can have nested fields and arrays. Collections group related documents, and databases contain multiple collections.

Which is more flexible - SQL or MongoDB? and why.

the choice between SQL and MongoDB depends on the specific needs of the application. SQL databases provide strong consistency and are suitable for structured, relational data, while MongoDB offers more flexibility in handling unstructured or evolving data models. The decision should consider factors such as data complexity, relationships, and the application's scalability and development requirements.

What is the disadvantage of a NoSQL database?

NoSQL databases lack a standardized query language like SQL. Each database type may have its own query language, making it less consistent and requiring developers to learn and adapt to different syntaxes.

### Resourses

[SQL vs NoSQL Database Differences](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool)

[ChatGPT](https://chat.openai.com/)
