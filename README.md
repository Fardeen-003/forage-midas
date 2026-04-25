# 💳 Midas Transaction Processing System

## 🚀 Overview
A real-time transaction processing system built using **Spring Boot and Apache Kafka**.  
This project simulates a backend system used in financial services to process streaming transaction data, validate balances, and update accounts.

Developed as part of the JPMorgan Chase Software Engineering Virtual Experience (Forage).

---

## 🏗️ System Architecture

Kafka → Listener → Business Logic → Database → REST API

- Kafka Producer sends transaction events
- Kafka Consumer processes transactions in real-time
- Spring Boot handles validation and business logic
- H2 Database stores users and transaction records
- External Incentive API provides bonus amounts
- REST API exposes user balances

---

## ⚙️ Tech Stack

- Java (Spring Boot)
- Apache Kafka
- Spring Data JPA
- H2 Database
- REST APIs (RestTemplate)
- Maven

---

## 🔑 Features

### 🔹 Real-Time Transaction Processing
- Consumes Kafka messages
- Processes financial transactions

### 🔹 Business Logic Validation
- Validates sender & recipient
- Prevents invalid transactions

### 🔹 Incentive API Integration
- Calls external API (`localhost:8080/incentive`)
- Adds incentive to recipient balance

### 🔹 Database Persistence
- Stores user and transaction data using JPA

### 🔹 REST API
Endpoint:
