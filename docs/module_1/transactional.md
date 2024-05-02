# Transactional data processing

A transactional system records **transactions** that encapsulate specific events that the organization wants to track. 

Transactional systems are often high-volume, sometimes handling many millions of transactions in a single day. The data being processed has to be accessible very quickly. The work performed by transactional systems is often referred to as **Online Transactional Processing (OLTP)**.

OLTP solutions rely on a database system in which data storage is **optimized for both read and write operations** in order to support transactional workloads in which data records are created, retrieved, updated, and deleted (often referred to as CRUD operations). These operations are applied transactionally, in a way that ensures the **integrity** of the data stored in the database. 

OLTP systems enforce transactions that support so-called ACID semantics:
- **Atomicity**: each transaction is treated as a single unit, which succeeds completely or fails completely.
- **Consistency**: transactions can only take the data in the database from one valid state to another. 
- **Isolation**: concurrent transactions cannot interfere with one another, and must result in a consistent database state. 
- **Durability**: when a transaction has been committed, it will remain committed.

OLTP systems are typically used to support live applications that process business data often referred to as line of business (LOB) applications.

