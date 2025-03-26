# DevOps-Driven AI System with Real-Time Database Interaction

## Overview
This project demonstrates a cutting-edge DevOps implementation of an AI system interacting with a MySQL database. It incorporates:

- **Apache Kafka** for real-time messaging.
- **ELK Stack (Elasticsearch, Logstash, Kibana)** for monitoring and log management.
- **Prometheus** for metrics collection and alerting.
- **Grafana** for visualization.

## Architecture
1. **MySQL**: Acts as the primary database storing application data.
2. **Apache Kafka**: Handles real-time data streaming.
3. **ELK Stack**: Captures logs from Kafka and MySQL for observability.
4. **Prometheus**: Collects metrics for Kafka, MySQL, and system health.
5. **Grafana**: Visualizes metrics for real-time monitoring.

## Components
### 1. MySQL
- Database for storing transactional data.
- Credentials are securely injected through environment variables.

### 2. Apache Kafka
- Broker for real-time messaging.
- Works with Zookeeper for managing configuration.

### 3. ELK Stack
- Elasticsearch for log storage.
- Logstash for log processing.
- Kibana for log visualization.

### 4. Prometheus
- Collects metrics for system health and performance.
- Uses a YAML configuration for scraping targets.

### 5. Grafana
- Connects to Prometheus for metric visualization.

## Prerequisites
- Docker & Docker Compose installed.
- Ports 3300, 9092, 5601, 9200, 9090, and 3000 open.

## How to Run
1. **Clone the Repository**
```bash
git clone <repository-url>
cd <repository-folder>
```

2. **Set Environment Variables**
Replace placeholders in `docker-compose.yml` and `mysql_dockerfile`.

3. **Start the Services**
```bash
docker-compose up -d
```

4. **Access the Services:**
- **MySQL:** `localhost:3300`
- **Kafka:** `localhost:9092`
- **Kibana:** `localhost:5601`
- **Prometheus:** `localhost:9090`
- **Grafana:** `localhost:3000`

## Observability and Monitoring
- **Kafka Logs:** Visible in Kibana.
- **Prometheus:** Metric scraping and alerting.
- **Grafana:** Custom dashboards for performance metrics.

## Conclusion
This project showcases how to integrate real-time messaging, metrics collection, and log management in a DevOps environment, emphasizing scalability, observability, and automation.
