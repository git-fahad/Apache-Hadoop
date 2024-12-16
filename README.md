# Apache-Hadoop
This repository contains Hadoop concepts and a project

# Hadoop: Architecture, Components, and Data Engineering Usage

## 1. Overview of Hadoop
Hadoop is an open-source framework for distributed storage and processing of large datasets across clusters of computers. It uses a simple programming model and is designed to scale from a single server to thousands of machines.

---

## 2. Hadoop Architecture
Hadoop has a master-slave architecture:
- **Master Node**: Manages resources and job scheduling.
- **Slave Nodes**: Store data and perform computations.

### Key Components
1. **Hadoop Distributed File System (HDFS)**: A distributed storage system.
2. **MapReduce**: A processing framework for parallel computations.
3. **YARN**: A resource management layer.
4. **Hadoop Common**: Utilities supporting other Hadoop modules.

---

## 3. Components Explained

### HDFS
- **Role**: Stores large datasets across multiple nodes.
- **Key Features**:
  - Write-once-read-many pattern.
  - Data is divided into blocks and replicated for fault tolerance.
- **Components**:
  - **NameNode**: Tracks metadata (file names, directories, blocks).
  - **DataNode**: Stores actual data blocks.

### MapReduce
- **Role**: Processes data in parallel using the Map and Reduce phases.
- **Workflow**:
  1. **Map Phase**: Processes input data and outputs key-value pairs.
  2. **Shuffle and Sort**: Groups and sorts the key-value pairs.
  3. **Reduce Phase**: Aggregates results based on keys.

### YARN (Yet Another Resource Negotiator)
- **Role**: Allocates resources and schedules jobs.
- **Components**:
  - **Resource Manager**: Manages resources globally.
  - **Node Manager**: Manages resources locally on nodes.
  - **Application Master**: Coordinates applications.

### Hadoop Common
- Provides libraries and utilities required by Hadoop's other modules.

---

## 4. Hadoop in Data Engineering

### Use Cases
- **Data Storage**: HDFS is used to store structured, semi-structured, and unstructured data.
- **Batch Processing**: MapReduce enables processing large volumes of data in batches.
- **ETL Processes**:
  - **Extract**: Read data from various sources (databases, logs).
  - **Transform**: Clean, format, and aggregate data.
  - **Load**: Store data in data warehouses or other systems.
- **Integration with Tools**:
  - **Hive**: SQL-like querying on HDFS.
  - **Pig**: Scripting for data transformations.
  - **HBase**: NoSQL database on HDFS.
  - **Spark**: In-memory processing for faster computations.
