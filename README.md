# RAGBot Starter

This project is a starter for creating a chatbot using MySQL, Kafka, MCP Server, and Prometheus. It's designed to be easy to deploy and use, with a focus on performance and usability.

## Features
- **MySQL Integration:** Store and retrieve data from your MySQL database with ease.
- **Kafka Integration:** Leverage Kafka for real-time messaging.
- **MCP Server:** Interact with your MCP server for processing.
- **Prometheus Integration:** Collect metrics and enable alerting for system health.
- **Custom Interface:** A simple, customizable chat interface for user interaction.

## Getting Started

### Prerequisites
- A running **MySQL** server.
- A working **Kafka** setup.
- An **MCP Server** running.
- **Prometheus** for metrics collection.

## Deployment

Deploy the chatbot system using Docker Compose:

```bash
docker-compose up -d
```

Ensure you have configured your **MySQL**, **Kafka**, **MCP Server**, and **Prometheus** services properly.

## Local Development

1. Clone this repository to your local machine.
2. Install dependencies by running:

```bash
npm install
```

3. Set up the following environment variables in your IDE or `.env` file:

```env
MYSQL_HOST=<INSERT_MYSQL_HOST>
MYSQL_USER=<INSERT_MYSQL_USER>
MYSQL_PASSWORD=<INSERT_MYSQL_PASSWORD>
MYSQL_DATABASE=<INSERT_MYSQL_DATABASE>

KAFKA_BROKER=<INSERT_KAFKA_BROKER>
MCP_SERVER_URL=<INSERT_MCP_SERVER_URL>
PROMETHEUS_URL=<INSERT_PROMETHEUS_URL>
```

4. Start the services with:

```bash
npm run dev
```

## Running the Project

To start the development server, run:

```bash
npm run dev
```

Open `http://localhost:3000` to view the chatbot in your browser.

## Monitoring and Logging
- **Prometheus** collects metrics and provides real-time alerting.
- **Kafka** enables real-time messaging for chat logs.
- **MCP Server** processes and responds to specific requests.

## Customization
Modify the chatbot interface or backend to suit your specific business needs.
