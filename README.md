# mongodbinterviewquestion

## Q - 1 Mongo db
- MongoDB is a cross-platform document-based database. Categorized as a NoSQL database, MongoDB avoids the conventional table-oriented relational database structure in support of the JSON-like documents with the dynamic schemas, making the data integration in specific kinds of applications quicker and simpler

## Q - 2 Features:-
Document Oriented and NoSQL database.
Supports Aggregation
Uses BSON format
Sharding (Helps in Horizontal Scalability)
Supports Ad Hoc Queries
Schema Less
Capped Collection
Indexing (Any field in MongoDB can be indexed)
MongoDB Replica Set (Provides high availability)
Supports Multiple Storage Engines

## SQL vs NOSQL

## Vertical vs Horizantal scaling

- SQL are vertical scalable This means that you can increase the load on a single server by increasing things like RAM, CPU or SSD
- NoSQL databases are horizontally scalable. This means that you handle more traffic by sharding, or adding more servers in your NoSQL database

## JSON VS BSON
- BSON is a binary encoded Javascript Object Notation (JSON)—a textual object notation widely used to transmit and store data across web based applications.
- BSON encodes type and length information, too, making it easier for machines to parse.
- BSON stands for Binary Javascript Object Notation. It is a binary-encoded serialization of JSON documents. BSON has been extended to add some optional non-JSON-native data types, like dates and binary data.

## Advantages of BSON:-
- Lightweight and Traversable
BSON is lightweight: This makes it possible for a large amount of data to be stored in BSON file format. Additionally, BSON files are easily stored and sent through the network, making them perfect for storing and sending data.

- efficient
- additonal data types


## Covered Query:-

Covered Query
- A covered query is a query that can be satisfied entirely using an index and does not have to examine any documents. An index  covers
 a query when all of the following apply:
  - all the fields in the query are part of an index, and
  - all the fields returned in the results are in the same index.

## What is the importance of profiler in MongoDB?
- MongoDB contains the database profiler that shows the performance characteristics of every operation against the database. Through the profiler, we can identify the queries that are slower than they should be and use this data to determine when we require an index.

## Join
- can do by $lookup operator to perform join with a collection.

## Some Commands:-
- **mongodump** - used to create a mongodb backup
- **mongorestore** - used to restore the data from backup 

## Aggregation:-
- $group - used to aggregate the results.

## Explain Capped Collection?
- In MongoDB, the Capped collection is a special kind of collection. This indicates that in this collection, we can restrict the collection size. Syntax of Capped - - - Collection is as follows:
  - Collection_Name: This field is the collection name that we create as the capped collection.
  - Capped: Capped is a boolean field; it is true if we create a capped collection. By default, its value is false.
  - auto indexed: It is a boolean flag that we use for auto-indexing. If this flag is true, indexes will be created automatically. If the flag is false, indexes will not be created automatically.
  - Size: Size is the parameter that represents the maximum amount of documents in bytes. It is the required field in the context of capped collections.
  - Max: Max is the parameter that represents the highest number of documents that permit the collection. 

## Save vs insert:-
- save - when having an id specified it replaces the documents with given id with the new document. when not provided id it just do simple insertion.
- insert - when having an id specified it gives an error as id already exists, while without id it simply do an insertion.

## Problem with find():-
- It will keep on searching the entire collections even if the document match has been found.



