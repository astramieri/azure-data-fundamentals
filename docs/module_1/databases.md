# Explore databases

A database is used to define a central system in which data can be stored and queried.

## Relational databases

Relational databases are commonly used to store and query structured data. 

The data is stored in **tables** that represent entities. Each instance of an entity is assigned a **primary key** that uniquely identifies it. Primary keys are used to reference the entity instance in other tables. 

The use of keys to reference data entities enables a relational database to be **normalized** which in part means the elimination of duplicate data values. 

The tables are managed and queried using **Structured Query Language (SQL)**, which is based on an ANSI standard, so it's similar across multiple database systems.

## Non-relational databases

Non-relational databases are data management systems that don’t apply a relational schema to the data. They are often referred to as NoSQL database, even though some support a variant of the SQL language.

There are four common types of non-relational database commonly in use:
- **key-value databases**
    - each record consists of a unique key and an associated value (which can be in any format)
- **document databases**
    - a specific form of key-value database in which the value is a JSON document (which the system is optimized to parse and query)
- **column-family databases**
    - they store tabular data comprising rows and columns, but you can divide the columns into groups known as column-families
- **graph databases**
    - they store entities as nodes with links to define relationships between them
