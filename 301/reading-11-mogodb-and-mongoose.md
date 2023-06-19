# MongoDB and Mongoose

## SQL vs NoSQL

Fill in the chart below with five differences between SQL and NoSQL databases:

|SQL | NoSQL|
|----|------|
|Table-based|Document-based|
|predefined schema|dynamic schema|
|vertically scalable|horizontally scalable|
|heavy duty transactional type app|Not as robust for heavy duty transactions|
|more supported|for some, relys on the community support

What kind of data is a good fit for an SQL database?

Data with well-defined structures and relationships, such as customer information, orders, and payments in an e-commerce platform.

Give a real world example.

An Online Shop:
Data being stored like customer information, order details all can be organized in structured tables

What kind of data is a good fit a NoSQL database?

Unstructured or semi-structured data, like user-generated content on social media platforms or data from IoT devices.

Give a real world example.

Social Media:
good fit for handling user-generated content. following relationships between all content, likes and profiles. Most things are varying but format.

Which type of database is best for hierarchical data storage?

NoSQL databases are ideal for storing hierarchical data with parent-child relationships, as they allow for easy organization and retrieval.

Which type of database is best for scalability?

NoSQL databases are better suited for handling large-scale applications and high traffic because they can scale horizontally by adding more servers to the database system.

## SQL NoSQL (video)

What does SQL stand for?

Structured Query Language

What is a relational database?

Organizes data into tables with predefined relationships between them. Established through keys, primary and foreign keys.

What type of structure does a relational database work with?

Works with a table structure, data is stored in tables   and they are made up of rows (records) and columns (fields) that define the attributes of the data.

What is a ‘schema’?

Schema is how the database is structured and organized. It is a blueprint  for how the data is stored and accessed in the database

What is a NoSQL database?

They are flexible and scalable in the data storage. they don't rely on a fixed schema. They can handle various data formats, such as key-value pairs, documents, columnar, or graph-based models

How does it work?

They work by using different data models and storage mechanisms depending on the specific type of NoSQL database. No tables here. just documents in a collection that resemble tables but looks like Json data.

What is inside of a MongoDB database?

databases of collections, which is stored in a collections. Each collection has indivial documents that look like Json

Which is more flexible - SQL or MongoDB? and why.

MongoDB offers more flexibility than traditional SQL databases. With MongoDB, you can easily use or change the data structure by adding or modifying fields within documents, without the need to alter the entire schema. This flexibility allows forsome complex data models, which can be advantageous in certain scenarios

What is the disadvantage of a NoSQL database?

One disadvantage of NoSQL databases is the lack of strict data consistency compared to SQL databases. NoSQL databases prioritize availability and scalability, which means they may sacrifice strict consistency. In some cases, this can lead to data inconsistencies or eventual consistency, where updates may not be immediately reflected across all nodes in a distributed database system. This trade-off is made to achieve high scalability and performance, but it might not be suitable for applications that require strong data consistency guarantees.

## Things I want to know more about

## References

[The Geek Stuff - SQL vs NoSQL Database Differences Explained with few Example DB](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool)

[SQL vs NoSQL or MySQL vs MongoDB](https://www.youtube.com/watch?v=ZS_kXvOeQ5Y)
