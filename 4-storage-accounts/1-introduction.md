# Azure Storage and Categories

Azure Storage is a service that you can use to store files, messages, tables, and other types of information. You use Azure storage for applications like file shares. Developers use Azure storage for working data. Working data includes websites, mobile apps, and desktop applications. Azure storage is also used by IaaS virtual machines, and PaaS cloud services. You can generally think of Azure storage in three categories.

- <strong>Storage for Virtual Machines:</strong> includes disks and files. Disks are persistent block storage for Azure IaaS virtual machines. Files are fully managed file shares in the cloud.

- <strong>Unstructured Data:</strong> includes Blobs and Data Lake Store. Blobs are highly scalable, REST-based cloud object store. Data Lake Store is Hadoop Distributed File System (HDFS) as a service.

- <strong>Structured Data:</strong> includes Tables, Cosmos DB, and Azure SQL DB. Tables are a key/value, autoscaling NoSQL store. Cosmos DB is a globally distributed database service. Azure SQL DB is a fully managed database-as-a-service built on SQL.

# Azure Storage Tier Performance

- <strong>Standard storage accounts</strong> are backed by magnetic drives (HDD) and provide the lowest cost per GB. Use Standard storage for applications that require bulk storage or where data is infrequently accessed.

- <strong>Premium storage accounts</strong> are backed by solid-state drives (SSD) and offer consistent low-latency performance. Use Premium storage for Azure virtual machine disks with I/O-intensive applications, like databases.

# Azure Storage Anatomy

Blob storage offers three types of resources:

- <strong>Storage Accounts:</strong> provides a unique namespace in Azure for your data. The combination of the account name and the blob storage endpoint forms the base address for the objects in your storage account.

<code>For example: https://mystorage.blob.core.windows.net</code>

- <strong>Container:</strong> a container organizes a set of blobs, similar to a directory in a file system. A storage account can include an unlimited number of containers, and a container can store an unlimited number of blobs.

- <strong>Blob:</strong>

    - <strong>Block blobs:</strong> store text and binary data. Block blobs are made up of blocks of data that can be managed individually. Block blobs can store up to about 190.7 TiB.

    - <strong>Append blobs:</strong> are made up of blocks like block blobs, but are optimized for append operations. Append blobs are ideal for scenarios such as logging data from virtual machines.

    - <strong>Page blobs:</strong> store random access files up to 8 TiB in size. Page blobs store virtual hard drive (VHD) files and serve as disks for Azure virtual machines. For more information about page blobs, see Overview of Azure page blobs