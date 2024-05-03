# Azure Stream Analytics

**Azure Stream Analytics** is a service for complex event processing and analysis of streaming data. 

Azure Stream Analytics is used to:
- **ingest data** from an input, such as an Azure Event Hub, Azure IoT Hub, or Azure Storage blob container
- **process data** by using a query to select, project, and aggregate data values
- **write the results** to an output, such as Azure Data Lake Gen 2, Azure SQL Database, Azure Synapse Analytics, Azure Functions, Azure Event Hub, Microsoft Power BI, or others

Once started, **a Stream Analytics query runs perpetually**, processing new data as it arrives in the input and storing results in the output.

Azure Stream Analytics is a great technology choice when you need to continually capture data from a streaming source, filter or aggregate it, and send the results to a data store or downstream process for analysis and reporting.

The easiest way to use Azure Stream Analytics is to create a **Stream Analytics job** in an Azure subscription, configure its input(s) and output(s), and define the query that the job will use to process the data. The query is expressed using structured query language (SQL) syntax, and can incorporate static reference data from multiple data sources to supply lookup values that can be combined with the streaming data ingested from an input.

If your stream process requirements are complex or resource-intensive, you can create a **Stream Analysis cluster**, which uses the same underlying processing engine as a Stream Analytics job, but in a dedicated tenant (so your processing isn't affected by other customers) and with configurable scalability that enables you to define the right balance of throughput and cost for your specific scenario.