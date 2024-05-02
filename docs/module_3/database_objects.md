# Database objects

In addition to tables, a relational database can contain other structures that help to optimize data organization, encapsulate programmatic actions, and improve the speed of access. 

## View

A **view** is a virtual table based on the results of a SELECT query. 

## Stored Procedure

A **stored procedure** defines SQL statements that can be run on command. Stored procedures are used to encapsulate programmatic logic in a database for actions that applications need to perform when working with data.

# Index

An **index** helps you search for data in a table. An index consumes storage space, and each time you insert, update, or delete data in a table, the indexes for that table must be maintained. This additional work can slow down insert, update, and delete operations.

An index can be:
- **Clustered**
    - Clustered indexes sort and store the data rows in the table or view based on their key values
    - These key values are the columns included in the index definition
    - There can be only one clustered index per table, because the data rows themselves can be stored in only one order
    - The only time the data rows in a table are stored in sorted order is when the table contains a clustered index
    - When a table has a clustered index, the table is called a **clustered table**
- **Non-clustered**
    - Nonclustered indexes have a structure separate from the data rows
    - A nonclustered index contains the nonclustered index key values and each key value entry has a pointer to the data row that contains the key value
    - The pointer from an index row in a nonclustered index to a data row is called a *row locator*