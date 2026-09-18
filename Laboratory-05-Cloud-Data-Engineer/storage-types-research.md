# Cloud Storage Types Research

Cloud storage can be divided into three common types: Block Storage, File Storage, and Object Storage. Each type is designed for different purposes and workloads.

| Storage Type       | Description                                                                                                       | Primary Use Case                                                                           | Cloud Provider Example |
| ------------------ | ----------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------ | ---------------------- |
| **Block Storage**  | Stores data in fixed-size blocks that can be managed by an operating system like a virtual hard drive.            | Best for virtual machines, databases, and applications that need fast disk access.         | AWS EBS                |
| **File Storage**   | Stores data as files organized into folders and directories that can be accessed by multiple users or systems.    | Best for shared files, documents, and applications that need a common file system.         | AWS EFS                |
| **Object Storage** | Stores data as objects together with metadata and a unique identifier inside a storage container called a bucket. | Best for images, videos, backups, documents, and other large amounts of unstructured data. | AWS S3                 |

## Why Object Storage for the Client?

Object Storage is a good choice for the client's photo-sharing application because it is designed to store large amounts of unstructured data such as images. It can also scale easily as the number of uploaded photos grows without requiring the same type of storage management as a traditional hard drive.

