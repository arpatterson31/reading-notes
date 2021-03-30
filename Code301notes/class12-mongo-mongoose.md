# Readings: Mongo and Mongoose

## Article - SQL vs NoSQL Database Differences

### SQL (structured query language)

- Relational Database (RDBMS)
- table based databases - data in rows of data
- predefined schema (the organization of data as a blueprint of how the database is constructed)
- verticially scalable
- good fit for complex query
- not good for hierarchical data storage
- great for heavy duty transactional type applications-more stable and promises integrity of the data
- emphasizes on Atomicity, Consistency, Isolation, Durability (ACID)
- EXAMPLES: MySql, Oracle, Sqlite, Postgres and MS-SQL

### NoSQL

- Non-Relational or distributed database
- Document based, key-value pairs, graph databases or wide-column stores
- dynamic schema for unstructured data
- horizontally scalable
- not a good fit for complex queries
- great for hierarchical data storage - great for big data
- not great for heavy duty transactional type applications
- emphasizes on Consistency, Availability, Partition tolerance (CAP)
- EXAMPLES: MongoDB, BigTable, Redis, RavenDb, Cassandra, Hbase, Neo4j, and CouchDb

#### MongoDB

- Benefits and Strengths
  - Speed
  - Scalability
  - Manageable
  - Dynamic Schema - flexibility to evolve your data schema without modifying existing data

## Article - NoSQL Data Modeling Techniques

- NoSQL data modeling starts from the application specific queries as apposed to relational modeling
- NoSQL data modeling requires a deeper understanding of data structures and algorithms

### Principles of NoSQL data modeling

1. Denormalization - copying the same data into multiple docs or tables to simplify/optimize query processing
2. Aggregates - key-value stores, BigTable, or document database
3. Application Side Joins - joins are rarely supported in NoSQL solutions

### Modeling Techniques

1. Atomic Aggregates - allow one to store a single business entity as one document, row or key-value pair and update it atomically
2. Enumerable Keys - unordered key-value data that allows entries to be partitioned across multiple servers by hashing the keys
3. Dimensionality Reduction - allows one to map multidimensional data to a key-value model or other non-multidimensional models
4. Index Table - allows one to take advantage of indexes in stores that do not support indexes internally
5. Composite Key Index - allows one to build a kind of multidimensional index which is fundamentally similar to dimensionally reduction technique
6. Aggregation with Composite Keys 
7. Inverted Search - Direct Aggreation - data procesesing pattern

### Hierarchy Modeling techniques

1. Tree Aggregation
2. Adjaceny Lists
3. Materialized Paths
4. Nested Sets
5. Nested Documents Flattening
6. Batch Graph Processing

##### Bookmark

- [mongoose api](https://mongoosejs.com/docs/api.html#Model)
