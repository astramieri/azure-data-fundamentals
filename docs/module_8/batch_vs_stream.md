# Understand batch and stream processing

Data processing is simply the conversion of raw data to meaningful information through a process. 

There are two general ways to process data:
- **batch processing** in which multiple data records are collected and stored before being processed together in a single operation
- **stream processing** in which a source of data is constantly monitored and processed in real time as new data events occur

## Batch Processing

In batch processing, newly arriving data elements are collected and stored, and the whole group is processed together as a batch. 

Exactly when each group is processed can be determined in a number of ways. For example, you can process data based on a scheduled time interval (for example, every hour), or it could be triggered when a certain amount of data has arrived, or as the result of some other event.

A real world example of batch processing is the way that credit card companies handle billing. The customer doesn't receive a bill for each separate credit card purchase but one monthly bill for all of that month's purchases.

**Advantages** of batch processing include:
- large volumes of data can be processed at a convenient time
- it can be scheduled to run at a time when computers or systems might otherwise be idle, such as overnight, or during off-peak hours

**Disadvantages** of batch processing include:
- the time delay between ingesting the data and getting the results
- all of a batch job's input data must be ready before a batch can be processed
- problems with data, errors, and program crashes that occur during batch jobs bring the whole process to a halt

## Stream processing

In stream processing, each new piece of data is processed when it arrives. 

Unlike batch processing, there's no waiting until the next batch processing interval. Data is processed as individual units in real-time rather than being processed a batch at a time. Stream data processing is beneficial in scenarios where new, dynamic data is generated on a continual basis.

A real world example of batch processing is the way a financial institution tracks changes in the stock market in real time, computes value-at-risk, and automatically rebalances portfolios based on stock price movements.

Stream processing is ideal for **time-critical operations that require an instant real-time response**. 

## Understand differences between batch and streaming data

| | Batch | Stream |
| - | - | - |
| **Data Scope** | Batch processing can process all the data in the dataset. | Stream processing typically only has access to the most recent data received, or within a rolling time window (e.g. the last 30 seconds). | 
| **Data Size** | Batch processing is suitable for handling large datasets efficiently. | Stream processing is intended for individual records or micro batches consisting of few records. |
| **Performance** | The latency (*) for batch processing is typically a few hours. | Stream processing typically occurs immediately, with latency (*) in the order of seconds or milliseconds. |
| **Analysis** | You typically use batch processing to perform complex analytics. | Stream processing is used for simple response functions, aggregates, or calculations such as rolling averages. |

(*) *Latency* is the time taken for the data to be received and processed. 

## Combine batch and stream processing

Many large-scale analytics solutions include **a mix of batch and stream processing**, enabling both historical and real-time data analysis. 

It's common for stream processing solutions to capture real-time data, process it by filtering or aggregating it, and present it through real-time dashboards and visualizations, while also persisting the processed results in a data store for historical analysis alongside batch processed data.

Even when real-time analysis or visualization of data is not required, streaming technologies are often used to capture real-time data and store it in a data store for subsequent batch processing.

Commonly used solution architectures for combined batch and stream data processing include *lambda* and *delta architectures*. 