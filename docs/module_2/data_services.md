# Identify data services

**Microsoft Azure** is a cloud platform that powers the applications and IT infrastructure for some of the world's largest organizations. It includes many services to support cloud solutions, including transactional and analytical data workloads.

## Azure SQL

Azure SQL is the collective name for a family of **relational database solutions** based on the **Microsoft SQL Server** database engine. 

Specific Azure SQL services include:
- **Azure SQL Database**: a fully managed platform-as-a-service (PaaS) database hosted in Azure
- **Azure SQL Managed Instance**: a hosted instance of SQL Server with automated maintenance, which allows more flexible configuration than Azure SQL DB but with more administrative responsibility for the owner
- **Azure SQL VM**: a virtual machine with an installation of SQL Server, allowing maximum configurability with full management responsibility

## Azure Database for open-source relational databases

Azure includes managed services for popular open-source relational database systems, including:
- **Azure Database for MySQL**: a simple-to-use open-source database management system that is commonly used in Linux, Apache, MySQL, and PHP (LAMP) stack apps
- **Azure Database for MariaDB**: a newer database management system, created by the original developers of MySQL (the database engine has since been rewritten and optimized to improve performance)
- **Azure Database for PostgreSQL**: a hybrid relational-object database (it enables you to store custom data types, with their own non-relational properties)

## Azure Cosmos DB

**Azure Cosmos DB** is a global-scale **non-relational (NoSQL) database** system that supports multiple application programming interfaces (APIs), enabling you to store and manage data as JSON documents, key-value pairs, column-families, and graphs.

## Azure Storage

**Azure Storage** is a core Azure service that enables you to store data in:
- **blob containers**: scalable, cost-effective storage for binary files
- **file shares**: network file shares such as you typically find in corporate networks
- **tables**: key-value storage for applications that need to read and write data values quickly

## Azure Data Factory

**Azure Data Factory** is an Azure service that enables you to define and schedule data pipelines to transfer and transform data. 

You can integrate your pipelines with other Azure services, enabling you to ingest data from cloud data stores, process the data using cloud-based compute, and persist the results in another data store.

Azure Data Factory is used by data engineers to build extract, transform, and load (ETL) solutions that populate analytical data stores with data from transactional systems across the organization.

## Azure Synapse Analytics

**Azure Synapse Analytics** is a comprehensive, unified Platform-as-a-Service (PaaS) solution for data analytics that provides a single service interface for multiple analytical capabilities, including:
- **Pipelines**: based on the same technology as Azure Data Factory.
- **SQL**: a highly scalable SQL database engine, optimized for data warehouse workloads
- **Apache Spark**: an open-source distributed data processing system that supports multiple programming languages and APIs, including Java, Scala, Python, and SQL
- **Azure Synapse Data Explorer**: a high-performance data analytics solution that is optimized for real-time querying of log and telemetry data using Kusto Query Language (KQL)

## Azure Databricks

**Azure Databricks** is an Azure-integrated version of the popular Databricks platform, which combines the Apache Spark data processing platform with SQL database semantics and an integrated management interface to enable large-scale data analytics.

## Azure HDInsight

**Azure HDInsight** is an Azure service that provides Azure-hosted **clusters** for popular Apache open-source big data processing technologies, including:
- **Apache Spark**: a distributed data processing system that supports multiple programming languages and APIs, including Java, Scala, Python, and SQL
- **Apache Hadoop**: a distributed system that uses MapReduce jobs to process large volumes of data efficiently across multiple cluster nodes
**Apache HBase**: an open-source system for large-scale NoSQL data storage and querying
- **Apache Kafka**: a message broker for data stream processing.

## Azure Stream Analytics

**Azure Stream Analytics** is a real-time stream processing engine that captures a stream of data from an input, applies a query to extract and manipulate data from the input stream, and writes the results to an output for analysis or further processing.

## Azure Data Explorer

**Azure Data Explorer** is a standalone service that offers the same high-performance querying of log and telemetry data as the Azure Synapse Data Explorer runtime in Azure Synapse Analytics

## Microsoft Purview

**Microsoft Purview** provides a solution for enterprise-wide data governance and discoverability. You can use Microsoft Purview to create a map of your data and track data lineage across multiple data sources and systems, enabling you to find trustworthy data for analysis and reporting.

## Microsoft Fabric

**Microsoft Fabric** is a unified Software-as-a-Service (SaaS) analytics platform based on open and governed lakehouse that includes functionality to support:
- Data ingestion and ETL
- Data lakehouse analytics
- Data warehouse analytics
- Data Science and machine learning
- Realtime analytics
- Data visualization
- Data governance and management