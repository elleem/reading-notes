## In Memory Storage
summarized from: https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool and https://www.youtube.com/watch?v=ZS_kXvOeQ5Y


### Things I Want to Know More About


### Questions

### nosqul vs sql
Fill in the chart below with five differences between SQL and NoSQL databases:

|SQL | NoSQL |
|-------|-------|	 
| a relational db | a non-relational or distributed db| 	 
| table based db | key-value, document, graph or wide-column based|
| predefined schema | dynamic schema for unstructured data|
| uses structured SQL queries | focused on collection of documents with varying syntax|
|	allows for a complex query intensive environment | don't have standard interfaces to perform complex queries|
 	 
What kind of data is a good fit for an SQL database?
high transaction based applications

Give a real world example.
transactional data.

What kind of data is a good fit a NoSQL database?
hierarchical data

Give a real world example.
JSON data

Which type of database is best for hierarchical data storage?
NoSQL, since it follows a key-value pair, similar to JSON

Which type of database is best for scalability?
SQL scales on one server via CPU, RAM, SSD (and has user support), NoSQL scales on multiple servers


### sql vs nosql

What does SQL stand for?
Structured Query Language

What is a relational database?
a db which has a relational model, representing the model as a collection of relations

What type of structure does a relational database work with?
tables (data bins)

What is a ‘schema’?
requirements for what goes into the table, which are defined by fields
every new entry/row is a record with these field values

What is a NoSQL database?
collections and documents, like JSON, that don't have to use the same schema

How does it work?
key and value pairs

What is inside of a Mongo database?
all the infromation in one data bin

Which is more flexible - SQL or MongoDB? and why.
Depends on the data you are storing: SQL allows for data consistency, NoSQL can be more flexible, but also difficult to update

What is the disadvantage of a NoSQL database?
difficult to update if you have data that is strongly related, and needs to be updated