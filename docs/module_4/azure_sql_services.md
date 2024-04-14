# Describe Azure SQL services and capabilities

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
    - A fully managed, highly scalable PaaS database service that is designed for the cloud. 
    - This service includes the core database-level capabilities of on-premises SQL Server
    - It supports *point-in-time restore*, enabling you to recover a database to the state it was in at any point in the past
    - It is a good option when you need to create a new application in the cloud
    - It is available as a *Single Database* or an *Elastic Pool*
    - You can also specify a *serverless* configuration
    - You can use the **Azure SQL Migration extension for Azure Data Studio** to detect compatibility issues with your databases that can impact database functionality in Azure SQL Database
- **Azure SQL Edge** 
    - A SQL engine that is optimized for Internet-of-things (IoT) scenarios that need to work with streaming time-series data