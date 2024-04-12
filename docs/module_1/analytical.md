# Explore analytical data processing

Analytical data processing typically uses read-only (or read-mostly) systems that store vast volumes of historical data or business metrics. Analytics can be based on a snapshot of the data at a given point in time, or a series of snapshots.

**Data lakes** are common in large-scale data analytical processing scenarios, where a large volume of file-based data must be collected and analyzed.

**Data warehouses** are an established way to store data in a relational schema that is optimized for read operations – primarily queries to support reporting and data visualization. 

**Data Lakehouses** are a more recent innovation that combine the flexible and scalable storage of a data lake with the relational querying semantics of a data warehouse. The table schema may require some denormalization of data in an OLTP data source (introducing some duplication to make queries perform faster).