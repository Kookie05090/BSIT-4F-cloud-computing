# Cloud Storage Types

## Comparison of Cloud Storage Types

| Storage Type | Description | Primary Use Case | Cloud Provider Example |
|---|---|---|---|
| Block Storage | Stores data in fixed-size blocks that can be attached to a computer or virtual machine like a hard drive. | Best used for operating systems, databases, and applications that need fast and consistent disk access. | AWS EBS |
| File Storage | Stores data as files organized into folders and directories that can be accessed through a shared file system. | Best used when multiple systems or users need to access and share files. | AWS EFS |
| Object Storage | Stores data as objects together with metadata and a unique identifier, making it suitable for large amounts of unstructured data. | Best used for images, videos, backups, documents, and other large collections of files. | AWS S3 |

## Why Object Storage is Suitable for the Client

Object Storage is a good choice for the client's photo-sharing application because it is designed to store large amounts of unstructured data such as images. It also makes it easier to organize and access millions of uploaded photos without storing them directly inside the web server.
