# Normalization

Normalization is a term used by database professionals for a schema design process that minimizes data duplication and enforces data integrity.

Instances of each entity are uniquely identified by an ID or other key value, known as a **primary key**; and when one entity references another, the primary key of the related entity is stored as a **foreign key**. 

Typically, a relational database management system (RDBMS) can enforce referential integrity to ensure that a value entered into a foreign key field has an existing corresponding primary key in the related table.

In some cases, a key (primary or foreign) can be defined as a composite key based on a unique combination of multiple columns.

Normalized databases are typically better optimized for write operations (INSERT, UPDATE, DELETE) rather than read operations. The normalization process involves organizing data to minimize redundancy and dependency, which can improve data integrity but may lead to more complex query structures for certain read operations.