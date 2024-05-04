# Azure SQL services and capabilities

**Azure SQL** is a collective term for a family of Microsoft SQL Server based database services in Azure:
- **SQL Server on Azure Virtual Machines (VMs)**
    - A virtual machine running in Azure with an installation of SQL Server
    - The use of a VM makes this option an IaaS solution
    - A great option for *lift and shift* migration to the cloud
- **Azure SQL Managed Instance**
    - A PaaS option that provides near-100% compatibility with on-premises SQL Server instances
    - The service includes automated software update management, backups, and other maintenance tasks
    - You can install multiple databases on the same instance
- **Azure SQL Database** 
    - A fully managed, highly scalable PaaS database service that is designed for the cloud
    - This service includes the core database-level capabilities of on-premises SQL Server
    - It supports *point-in-time restore*, enabling you to recover a database to the state it was in at any point in the past
    - It is a good option when you need to create a new application in the cloud
    - It is available as a *Single Database* or an *Elastic Pool*
    - You can also specify a *serverless* configuration
    - You can use the **Azure SQL Migration extension for Azure Data Studio** to detect compatibility issues with your databases that can impact database functionality in Azure SQL Database
- **Azure SQL Edge** 
    - A SQL engine that is optimized for Internet-of-things (IoT) scenarios that need to work with streaming time-series data

## Connectivity Architecture

When a connection from a server to an Azure SQL database, the client will connect to a **gateway that listen on port 1443**. Baes on the connection policiy the gateway will grant traffic and route access to the appropriate database.

The are three kinds of connection policies:
- **proxy**: intended for workloads connecting *outside* the Azure Network
- **redirect**: intended for workloads connecting *inside* the Azure Network
- **default**: based on workloads inside or outside the Azure Network

## SQL Server Authentication

During setup of SQL Server Database you must select an **authentication mode**:
- **Windows Authentication Mode** (recommended)
    - enables Windows Authentication and disables SQL Server Authentication
- **Mixed Mode**
    - enables both Windows Authentication and SQL Server Authentication

## Transparent Data Encryption (TDE)

Transparent Data Encryption (TDE) protects Azure SQL database, Azure Synapse Analytics, and Azure SQL Managed Instance against malicious offline activities by *encrypting the data at rest*.

## Azure SQL Database Firewall

The **Azure SQL Database firewall** lets you decide which IP addresses may or may not have access to either your Azure SQL Server or your Azure SQL database. 

When creating an Azure SQL Database, the firewall needs to be configured before anyone will be able to access the database. By default, no external access to your SQL Database will be allowed until you explicitly assign permission by creating a firewall rule.
 
## SQL Server Management Studio (SSMS)

SQL Server Management Studio (SSMS) is an integrated environment for managing any SQL infrastructure, from SQL Server to Azure SQL Database.

## Microsoft SQL Server Data Tools (SSDT)

SQL Server Data Tools (SSDT) is a modern development tool for building SQL Server relational databases, databases in Azure SQL, Analysis Services (AS) data models, Integration Services (IS) packages, and Reporting Services (RS) reports. 

With SSDT, you can design and deploy any SQL Server content type with the same ease as you would develop an application in Visual Studio.
