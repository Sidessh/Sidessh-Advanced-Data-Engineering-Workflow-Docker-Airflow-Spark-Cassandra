![image](https://github.com/user-attachments/assets/e42bde16-66c4-4112-9513-b9243fb29cee)

# **Real-Time Data Engineering Pipeline**

## **Overview**
This project demonstrates the implementation of a real-time data engineering pipeline leveraging modern tools and technologies to process, orchestrate, and store streaming and batch data. The architecture integrates **Apache Airflow**, **Apache Kafka**, **Apache Spark**, **Cassandra**, **PostgreSQL**, and **Docker** to deliver a scalable and efficient solution for data workflows.

---

## **System Architecture**
![System Architecture](link-to-your-diagram.png)

The pipeline consists of:
1. **Apache Kafka**: For real-time data streaming and message brokering.
2. **Apache Airflow**: For workflow orchestration and task automation.
3. **Apache Spark**: For distributed data processing.
4. **Cassandra**: For storing real-time processed data.
5. **PostgreSQL**: For batch data storage and querying.
6. **Docker**: For containerized deployment ensuring portability and scalability.

---

## **Key Features**
- **End-to-End Workflow Automation**: Orchestrated data flows using Airflow to manage dependencies and execution.
- **Real-Time Streaming**: Kafka enables low-latency data pipelines for streaming ingestion.
- **Distributed Processing**: Spark processes and transforms data at scale across multiple nodes.
- **Hybrid Storage**: Integration of Cassandra for real-time data and PostgreSQL for batch analytics.
- **Scalability and Portability**: Dockerized components for seamless deployment.

---

## **Setup and Installation**

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <repository-directory>
   ```

2. Ensure Docker and Docker Compose are installed.

3. Start the pipeline:
   ```bash
   docker-compose up -d
   ```

---

## **Data Flow**

1. **Data Generation**: A custom API generates raw data.
2. **Kafka**: Streams the data to various topics.
3. **Spark**: Consumes Kafka streams, processes the data, and writes outputs to Cassandra and PostgreSQL.
4. **Airflow**: Manages task dependencies and orchestrates workflows.
5. **Cassandra**: Stores processed real-time data for fast reads.
6. **PostgreSQL**: Stores batch data for analytical querying.

---

## **Technologies Used**
- **Orchestration**: Apache Airflow
- **Streaming**: Apache Kafka, Zookeeper
- **Processing**: Apache Spark
- **Storage**: Cassandra, PostgreSQL
- **Deployment**: Docker and Docker Compose
- **Monitoring**: Kafka Control Center

---
