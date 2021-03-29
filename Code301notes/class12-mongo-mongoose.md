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

1. Atomic Aggregates

##### Bookmark

- [mongoose api](https://mongoosejs.com/docs/api.html#Model)
