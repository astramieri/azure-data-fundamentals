# Azure Files

**Azure Files** is essentially a way to create cloud-based network shares, such as you typically find in on-premises organizations to make documents and other files available to multiple users. 

By hosting file shares in Azure, organizations can eliminate hardware costs and maintenance overhead, and benefit from high availability and scalable cloud storage for files.

You create Azure File storage in a Storage Account. Azure Files enables you to share up to 100 TB of data in a single storage account. This data can be distributed across any number of file shares in the account. 

The maximum size of a single file is 1 TB, but you can set quotas to limit the size of each share below this figure. Currently, Azure File Storage supports up to 2000 concurrent connections per shared file.

You can upload files to Azure File Storage using:
- Azure portal
- AzCopy utility
- Azure File Sync service

![Azure Files](azure_files.png)

## Azure Files Performance Tiers

Azure File Storage offers two performance tiers:
- **standard tier** uses hard disk-based hardware in a datacenter
- **premium tier** uses solid-state disks

The premium tier offers greater throughput, but is charged at a higher rate.

## Azure Files Sharing Protocols

Azure Files supports two common network file sharing protocols:
- **Server Message Block (SMB)** file sharing is commonly used across multiple operating systems (Windows, Linux, macOS)
- **Network File System (NFS)** shares are used by some Linux and macOS versions