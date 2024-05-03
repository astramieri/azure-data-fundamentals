# Data warehouse architecture

A large-scale data analytics architecture includes:
- **Data ingestion and processing**
    - Data from one or more transactional data stores, files, real-time streams, or other sources is loaded into a data lake or a relational data warehouse 
    - The data processing is often performed by distributed systems that can process high volumes of data in parallel using multi-node clusters
    - Data ingestion includes both **batch processing** of static data and **real-time processing** of streaming data
- **Data store**
    - Data stores for large scale analytics include relational data warehouses, file-system based data lakes, and hybrid architectures that combine features of data warehouses and data lakes (sometimes called data lakehouses or lake databases)
- **Data model**
    - It’s common to create one or more data models that pre-aggregate the data to make it easier to produce reports, dashboards, and interactive visualizations
    - The model encapsulates the relationships between data values and dimensional entities to support *drill-up and drill-down* analysis
- **Data visualization** 
    - Data analysts consume data from analytical models, and directly from analytical stores to create reports, dashboards, and other visualizations
    - The visualizations from the data show trends, comparisons, and key performance indicators (KPIs) for a business or other organization, and can take the form of printed reports, graphs and charts in documents or PowerPoint presentations, web-based dashboards, and interactive environments in which users can explore data visually