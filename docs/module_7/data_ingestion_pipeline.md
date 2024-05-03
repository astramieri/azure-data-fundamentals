# Data ingestion pipelines

On Azure, large-scale data ingestion is best implemented by creating **pipelines** that orchestrate ETL processes. 

You can create and run pipelines using **Azure Data Factory**, or you can use a similar pipeline engine in **Azure Synapse Analytics** or **Microsoft Fabric** if you want to manage all of the components of your data analytics solution in a unified workspace.

In either case, **pipelines consist of one or more activities that operate on data**. An input dataset provides the source data, and activities can be defined as a data flow that incrementally manipulates the data until an output dataset is produced. Pipelines can connect to external data sources to integrate with a wide variety of data services.