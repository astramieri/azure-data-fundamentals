# A general architecture for stream processing

At its simplest, a high-level architecture for stream processing looks like this:
1. An event generates some data
2. The generated data is captured in a streaming source for processing
    - The source may be a cloud folder, or a database table, or a queue
3. The event data is processed
4. The results of the stream processing operation are written to an output (or *sink*)
    - The output may be a file, a database table, a real-time visual dashboard, or another queue for further processing 

## Real-time analytics in Azure

Microsoft Azure supports multiple technologies that you can use to implement real-time analytics of streaming data, including:
- **Azure Stream Analytics**
    - A platform-as-a-service (PaaS) solution that you can use to define streaming jobs that ingest data from a streaming source, apply a perpetual query, and write the results to an output
- **Spark Structured Streaming**
    - An open-source library that enables you to develop complex streaming solutions on Apache Spark based services, including Azure Synapse Analytics, Azure Databricks, and Azure HDInsight
- **Azure Data Explorer**
    - A high-performance database and analytics service that is optimized for ingesting and querying batch or streaming data with a time-series element, and which can be used as a standalone Azure service or as an Azure Synapse Data Explorer runtime in an Azure Synapse Analytics workspace

## *Sources* for stream processing

The following services are commonly used to ingest data for stream processing on Azure:
- **Azure Event Hubs**
    - A data ingestion service that you can use to manage queues of event data, ensuring that each event is processed in order, exactly once
- **Azure IoT Hub**
    - A data ingestion service that is similar to Azure Event Hubs, but which is optimized for managing event data from Internet-of-things (IoT) devices
- **Azure Data Lake Store Gen 2**
    - A highly scalable storage service that is often used in batch processing scenarios, but which can also be used as a source of streaming data
- **Apache Kafka**
    - An open-source data ingestion solution that is commonly used together with Apache Spark

## *Sinks* for stream processing

The output from stream processing is often sent to the following services:
- **Azure Event Hubs**
    - Used to queue the processed data for further downstream processing
- **Azure Data Lake Store Gen 2** or **Azure blob storage**
    - Used to persist the processed results as a file
- **Azure SQL Database** or **Azure Synapse Analytics** or **Azure Databricks**
    - Used to persist the processed results in a database table for querying and analysis
- **Microsoft Power BI**
    - Used to generate real time data visualizations in reports and dashboards

