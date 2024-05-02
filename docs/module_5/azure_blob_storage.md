# Explore Azure Blob Storage

**Azure Blob Storage** is a service that enables you to store massive amounts of unstructured data as binary large objects (i.e. blobs) in the cloud. 

Blobs are an efficient way to store data files in a format that is optimized for cloud-based storage and applications can read and write them by using the Azure blob storage API.

In an **Azure Storage Account**, you store blobs in **containers**. A container provides a convenient way of grouping related blobs together. You control who can read and write blobs inside a container at the container level.

Within a container, you can organize blobs in a hierarchy of virtual folders, similar to files in a file system on disk. However *by default* these folders are simply a way of using a "/" character in a blob name to organize the blobs into namespaces. The **folders are purely virtual**, and you can't perform folder-level operations to control access or perform bulk operations.

Objects in Blob storage are accessible via:
- Azure Storage REST API
- Azure PowerShell
- Azure CLI
- Azure Storage client library

![Azure Blob Storage](azure_blob_storage.png)

## Types of blob data

Azure Blob Storage supports three different types of blob:
- **block**
    - they are best used to store discrete, large, binary objects that change infrequently
- **page**
    - a page blob is optimized to support random read and write operations
    - a page blob can hold up to 8 TB of data
    - Azure uses page blobs to implement virtual disk storage for virtual machines
- **append**: 
    - an append blob is a block blob optimized to support append operations
    - you can only add blocks to the end of an append blob
    - updating or deleting existing blocks isn't supported
    - the maximum size of an append blob is just over 195 GB

## Access tiers for blob data

Blob storage provides three access tiers, which help to balance access latency and storage cost:
- **Hot tier**
    - it is the default
    - it is used for blobs that are accessed frequently
- **Cool tier**
    - lower performance and reduced storage charges (compare to Hot tier)
    - it is used for blobs that are accessed infrequently
- **Archive tier**
    - it provides the lowest storage cost, but with increased latency
    - it is intended for historical data that mustn't be lost, but is required only rarely
    - blobs in the Archive tier are effectively stored in an **offline state** 

## Lifecycle Management Policies

A lifecycle management policy can automatically move a blob from Hot to Cool, and then to the Archive tier, as it ages and is used less frequently (policy is based on the number of days since modification). 

A lifecycle management policy can also arrange to delete outdated blobs.
