# What is Mongo DB?

MongoDB, the most popular NoSQL database, is an open-source document-oriented database. The term ‘NoSQL’ means ‘non-relational’. It means that MongoDB isn’t based on the table-like relational database structure but provides an altogether different mechanism for storage and retrieval of data. This format of storage is called BSON ( similar to JSON format).

A simple MongoDB document Structure:
```
{
  title: 'Geeksforgeeks',
  by: 'Harshit Gupta',
  url: 'https://www.geeksforgeeks.org',
  type: 'NoSQL'
} 
```
SQL databases store data in tabular format. This data is stored in a predefined data model which is not very much flexible for today’s real-world highly growing applications. Modern applications are more networked, social and interactive than ever. Applications are storing more and more data and are accessing it at higher rates.

Relational Database Management System(RDBMS) is not the correct choice when it comes to handling big data by the virtue of their design since they are not horizontally scalable. If the database runs on a single server, then it will reach a scaling limit. NoSQL databases are more scalable and provide superior performance. MongoDB is such a NoSQL database that scales by adding more and more servers and increases productivity with its flexible document model.

<img src="https://github.com/stormfireuttam/MongoDB/blob/main/01%20Introduction/Image01.jpg"/>

#  RDBMS vs MongoDB:


 -   RDBMS has a typical schema design that shows number of tables and the relationship between these tables whereas MongoDB is document-oriented. There is no concept of schema or relationship.
 -   Complex transactions are not supported in MongoDB because complex join operations are not available.
 -   MongoDB allows a highly flexible and scalable document structure. For example, one data document of a collection in MongoDB can have two fields whereas the other document in the same collection can have four.
 -   MongoDB is faster as compared to RDBMS due to efficient indexing and storage techniques.
 <img src="https://github.com/stormfireuttam/MongoDB/blob/main/01%20Introduction/document.jpg"/>

-   There are a few terms which are related in both the databases. What’s called Table in RDBMS is called a Collection in MongoDB. Similarly, a Tuple/Row is called a Document and A Column is called a Field. MongoDB provides a default ‘_id’ (if not provided explicitly) which is a 12 byte hexadecimal number which assures the uniqueness of every document. It is similar to the Primary key in RDBMS.

<img src="https://github.com/stormfireuttam/MongoDB/blob/main/01%20Introduction/collection.jpg"/>


# Features of MongoDB:

  - **Document Oriented:** MongoDB stores the main subject in the minimal number of documents and not by breaking it up into multiple relational structures like RDBMS. For example, it stores all the information of a computer in a single document called Computer and not in distinct relational structures like CPU, RAM, Hard disk, etc.
  - **Indexing:** Without indexing, a database would have to scan every document of a collection to select those that match the query which would be inefficient. So, for efficient searching Indexing is a must and MongoDB uses it to process huge volumes of data in very less time.
  - **Scalability:** MongoDB scales horizontally using sharding (partitioning data across various servers). Data is partitioned into data chunks using the shard key, and these data chunks are evenly distributed across shards that resides across many physical servers. Also, new machines can be added to a running database.
  - **Replication and High Availability:** MongoDB increases the data availability with multiple copies of data on different servers. By providing redundancy, it protects the database from hardware failures. If one server goes down, the data can be retrieved easily from other active servers which  also had the data stored on  them.
  - **Aggregation:** Aggregation operations process data records and return the computed results. It is similar to the GROUPBY clause in SQL. A few aggregation expressions are sum, avg, min, max, etc


# Where do we use MongoDB?

MongoDB is preferred over RDBMS in the following scenarios:

  -  Big Data: If you have huge amount of data to be stored in tables, think of MongoDB before RDBMS databases. MongoDB has built in solution for partitioning and sharding your database.
  -  Unstable Schema: Adding a new column in RDBMS is hard whereas MongoDB is schema-less. Adding a new field, does not effect old documents and will be very easy.
  -  Distributed data Since multiple copies of data  are stored across different servers, recovery of data is instant and safe even if there is a hardware failure.

# Language Support by MongoDB:

MongoDB currently provides official driver support for all popular programming languages like C, C++, C#, Java, Node.js, Perl, PHP, Python, Ruby, Scala, Go and Erlang.

# Installing MongoDB:

Just go to http://www.mongodb.org/downloads and select your operating system out of Windows, Linux, Mac OS X and Solaris. Detailed explanation about the installation of MongoDB is given on their site.

For Windows, a few options for the 64-bit operating systems drops down. When you’re running on Windows 7, 8 or newer versions, select Windows 64-bit 2008 R2+. When you’re using Windows XP or Vista then select Windows 64-bit 2008 R2+ legacy.


# Who’s using MongoDB?

MongoDB has been adopted as backend software by a number of major websites and services including EA, Cisco, Shutterfly, Adobe, Ericsson, Craigslist, eBay, and Foursquare.
