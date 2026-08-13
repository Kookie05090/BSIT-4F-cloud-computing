# Cloud Infrastructure Components

## 1. Compute Resources

### Purpose

Compute resources provide the processing power needed to run applications, services, and workloads. They include the CPU and memory used by a server.

### Importance in Cloud Computing

Compute resources are important because they allow cloud users to run applications without managing physical hardware directly. Cloud providers can provide different amounts of CPU and memory depending on the needs of the workload.

### Relation to the KillerCoda Environment

In the KillerCoda Ubuntu environment, the compute resources include the Intel Xeon CPU with 1 CPU core and 1.9 GiB of RAM. These resources allow the Linux server to run commands and applications.

## 2. Storage Resources

### Purpose

Storage resources are used to store the operating system, applications, files, and other data.

### Importance in Cloud Computing

Storage is important because cloud applications need a place to save and access data. Different types of cloud storage can be used depending on the required capacity and performance.

### Relation to the KillerCoda Environment

In the KillerCoda environment, the main storage device is `/dev/vda1` with a capacity of 19 GB. The system also has mounted file systems such as `/`, `/boot`, and `/boot/efi`.

## 3. Networking Resources

### Purpose

Networking resources allow devices, servers, and users to communicate with each other and access services.

### Importance in Cloud Computing

Networking is important because cloud services need connections between users, applications, servers, and other resources. It allows data to be transferred through networks and accessed over the internet.

### Relation to the KillerCoda Environment

In the KillerCoda Linux environment, networking is represented by the assigned IP addresses `172.30.1.2` and `172.17.0.1`. These addresses allow the server environment to communicate within its network.

## 4. Operating System

### Purpose

The operating system manages the hardware and software resources of a computer or server. It provides an environment where applications and services can run.

### Importance in Cloud Computing

Operating systems are important in cloud computing because cloud servers need software that manages computing resources and supports applications. Linux is commonly used for cloud servers because it is flexible and widely supported.

### Relation to the KillerCoda Environment

The KillerCoda environment uses Ubuntu 24.04.4 LTS with the Linux kernel version `6.8.0-136-generic`. The operating system manages the server's CPU, memory, storage, and networking resources.
