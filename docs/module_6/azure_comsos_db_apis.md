# Azure Cosmos DB APIs

Azure Cosmos DB is a fully managed and serverless distributed database for applications of any size or scale, with **support for both relational and non-relational workloads**. 

Developers can build and migrate applications fast using their preferred open source database engines, including PostgreSQL, MongoDB, and Apache Cassandra. 

When you provision a new Cosmos DB instance, **you select the database engine** that you want to use. 

The choice of engine depends on many factors including:
- the type of data to be stored
- the need to support existing applications
- the skills of the developers who will work with the data store

## Azure Cosmos DB for NoSQL

**Azure Cosmos DB for NoSQL** is Microsoft’s **native non-relational service** for working with the **document data model**. 

It manages data in JSON document format, and despite being a NoSQL data storage solution, uses SQL syntax to work with the data.

#### SQL Input 

    SELECT *
      FROM customers c
     WHERE c.id = "joe@litware.com"

#### JSON Output

    {
        "id": "joe@litware.com",
        "name": "Joe Jones",
        "address": {
            "street": "1 Main St.",
            "city": "Seattle"
        }
    }

## Azure Cosmos DB for MongoDB

**Azure Cosmos DB for MongoDB** enables developers to use MongoDB client libraries and code to work with data in Azure Cosmos DB.

MongoDB is a popular open source database in which **data is stored in Binary JSON (BSON) format**. 

MongoDB Query Language (MQL) uses **a compact object-oriented syntax** in which developers use objects to call methods. 

The MongoDB API is queried by using MongoDB Query Language (MQL). 

#### JavaScript Input

    db.products.find({id: 123})

#### JSON Output 

    {
        "id": 123,
        "name": "Hammer",
        "price": 2.99
    }

## Azure Cosmos DB for PostgreSQL

**Azure Cosmos DB for PostgreSQL** is a **native PostgreSQL globally distributed relational database** that automatically shards data to help you build highly scalable apps. 

You can start building apps on a single node server group, the same way you would with PostgreSQL anywhere else. As your app's scalability and performance requirements grow, **you can seamlessly scale to multiple nodes** by transparently distributing your tables. 

PostgreSQL is a relational database management system (RDBMS) in which you define relational tables of data.

## Azure Cosmos DB for Table

**Azure Cosmos DB for Table** is used to work with data in **key-value tables** similar to Azure Table Storage. 

It offers **greater scalability** and performance than Azure Table Storage and provides resiliency if an Azure region declines. 

The Table API is queried by using OData and LINQ queries.

## Azure Cosmos DB for Apache Cassandra

**Azure Cosmos DB for Apache Cassandra** is compatible with Apache Cassandra, which is a popular open source database that uses a column-family storage structure. 

Column families are tables, similar to those in a relational database, with the exception that it's not mandatory for every row to have the same columns.

The Cassandra API is queried by using SQL.

## Azure Cosmos DB for Apache Gremlin

**Azure Cosmos DB for Apache Gremlin** is used with data in a **graph structure** in which entities are defined as vertices that form nodes in connected graph.

The Gremlin API is queried by using Graph. 