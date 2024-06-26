# Platform-as-a-service (PaaS) solutions

On Azure, there are three main platform-as-a-service (PaaS) services that you can use to implement a large-scale analytics:
- Azure Synapse Analytics
- Azure Databricks
- Azure HDInsight

## Azure Synapse Analytics

Azure Synapse Analytics is a **unified end-to-end solution for large scale data analytics**. 

It brings together multiple technologies and capabilities, enabling you to combine the data integrity and reliability of a scalable high-performance SQL Server based relational data warehouse with the flexibility of a data lake and open-source Apache Spark.

It also includes native support for log and telemetry analytics with Azure Synapse Data Explorer pools, as well as built in data pipelines for data ingestion and transformation. 

All Azure Synapse Analytics services can be managed through a single interactive user interface called **Azure Synapse Studio**, which includes the ability to create interactive notebooks in which Spark code and markdown content can be combined. 

**Synapse SQL** is a distributed version of T-SQL designed for data warehouse workloads. It offers both serverless and dedicated resource models for unpredictable or predictable workloads.

Synapse Analytics is a great choice when you want to create a single, unified analytics solution on Azure.

## Azure Databricks

**Azure Databricks** is an Azure implementation of the popular Databricks platform. 

Databricks is a comprehensive data analytics solution built on Apache Spark, and offers native SQL capabilities as well as workload-optimized Spark clusters for data analytics and data science. 

Databricks provides an interactive user interface through which the system can be managed and data can be explored in interactive notebooks. 

Due to its common use on multiple cloud platforms, you might want to consider using Azure Databricks as your analytical store if you want to use existing expertise with the platform or if you need to operate in a multicloud environment or support a cloud-portable solution.

## Azure HDInsight

**Azure HDInsight** is an Azure service that supports multiple open-source data analytics cluster types. Although not as user-friendly as Azure Synapse Analytics and Azure Databricks, it can be a suitable option if your analytics solution relies on multiple open-source frameworks or if you need to migrate an existing on-premises Hadoop-based solution to the cloud.

## Polybase

Polybase is a **data virtualization feature** for SQL Server.

PolyBase enables your SQL Server instance to query data with T-SQL directly from different sources without separately installing client connection software.

PolyBase allows you to join data from a SQL Server instance with external data.
