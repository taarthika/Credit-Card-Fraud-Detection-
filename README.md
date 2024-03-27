# Real-Time Credit Card Fraud Detection System

## Introduction

This repository contains the implementation of a real-time credit card fraud detection system using Apache Kafka, Kafka Streams (KSQLDB), MongoDB, and Flink. The system is designed to ingest credit card transaction data, analyze it for suspicious patterns, and generate alerts in real-time.

## Setup and Installation

### Prerequisites

Ensure you have the following prerequisites installed on your system:

- Java
- Apache Kafka
- Kafka Streams (KSQLDB)
- MongoDB
- Python
- Faker library

Alternatively, you can use managed services from Confluent Cloud.

### Installation

Use the following pip command to install required Python libraries:

```bash
pip install kafka-python confluent-kafka ksql kafka-streams faker pyflink pymongo
```

Start a local Kafka cluster using Docker:

```bash
docker-compose up -d kafka zookeeper
```

## Usage

### Generate Data

Use the provided Python script to generate simulated credit card transactions.

### Real-time Fraud Detection with KSQLDB

Configure Kafka Connect to stream data from Kafka topics to KSQLDB.

Create a KSQLDB stream to consume transactions from Kafka.

Define KSQL queries for real-time processing of credit card transactions.

Implement queries to identify potential fraud patterns based on transaction characteristics.

Create a KSQL stream to detect fraudulent transactions.

### Store Data in MongoDB

Create a Python script using PyMongo to write flagged transactions to MongoDB.

### Real-time Analytics with Apache Flink

Create a Flink application to analyze flagged transactions in real-time.

Use Flink SQL for easier implementation.

## Reflect and Share

Summarize your learning experience, challenges faced, and insights gained. Document technical difficulties and possible best practices discovered in the process.

## Resources

- Confluent Cloud Documentation
- Apache Flink Stream Processing Exercise
- Deploying an ETL Pipeline using Flink SQL Exercise
- Credit Card Activity Tutorial
- Kafka Source/Sink with Apache Flink Table API
  
## Contributors

- Krishna Velamala
- Leela Sai Rahul
- Nivegna Lagdapati
- Harshitha Boddu

