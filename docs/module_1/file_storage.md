# Explore file storage

In most organizations, important data files are stored centrally in some kind of **shared file storage system**. Increasingly, that central storage location is hosted in the cloud, enabling cost-effective, secure, and reliable storage for large volumes of data.

## Delimited text files

Data is often stored in plain text format with specific *field delimiters* and *row terminators*. 

The most common format for delimited data is comma-separated values (CSV) in which fields are separated by **commas**, and rows are terminated by a **carriage return** or/and **new line**.

## JavaScript Object Notation (JSON)

JSON is a ubiquitous format in which a **hierarchical** document schema is used to define data **entities** (objects) that have multiple **attributes**. 

Each attribute might be an object (or a collection of objects), making JSON a flexible format that's good for both structured and semi-structured data.

## Extensible Markup Language (XML)

XML is a human-readable data format that was popular in the 1990s and 2000s. It's largely been superseded by the less verbose JSON format, but there are still some systems that use XML to represent data. XML uses tags enclosed in *angle-brackets* to define **elements** and **attributes**.

## Binary Large Object (BLOB)

Ultimately, all files are stored as **binary data** (1's and 0's), but in the human-readable formats discussed above, the bytes of binary data are mapped to printable characters (typically through a character encoding scheme such as ASCII or Unicode).

## Optimized file formats

While human-readable formats for structured and semi-structured data can be useful, they're typically not optimized for storage space or processing. 

Over time, some specialized file formats that enable compression, indexing, and efficient storage and processing have been developed.

Some common optimized file formats you might see include:
- **Avro** 
    - It is a row-based format created by Apache
    - Each record contains a header (stored as JSON) that describes the structure of the data in the record
    - The data is stored as binary information    
    - It is a good format for compressing data and minimizing storage and network bandwidth requirements
- **ORC (Optimized Row Columnar format)**
    - It organizes data into columns rather than rows
    - It was developed by HortonWorks for optimizing read and write operations in Apache Hive
    - An ORC file contains *stripes of data* 
    - A stripe holds the data for a column or set of columns
    - A stripe contains:
        - an index into the rows in the stripe
        - the data for each row
        - a footer that holds statistical information (count, sum, max, etc.) for each column
- **Parquet**
    - It is another columnar data format created by Cloudera and Twitter
    - A Parquet file contains *row groups*
    - Data for each column is stored together in the same row group
    - Each row group contains one or more chunks of data
    - It is specialized in storing and processing nested data types efficiently
    - It supports very efficient compression and encoding schemes