# .NET Microservices E-Commerce Platform

## 📌 Overview

This project demonstrates a scalable **e-commerce microservices architecture** built using **ASP.NET Core and .NET 8**. It showcases real-world backend engineering concepts such as **API Gateway, event-driven communication, distributed systems, and containerized deployments**.

The system is designed by leveraging a reference microservices architecture and extending it with custom implementations and enhancements to simulate **production-grade enterprise systems**.

---

## 🚀 Key Features

* Microservices architecture using **ASP.NET Core & C#**
* API Gateway implementation using **Ocelot**
* Event-driven communication with **RabbitMQ**
* Hybrid database architecture:

  * **SQL Server (Relational)**
  * **MongoDB & Redis (NoSQL)**
* Authentication & Authorization using **JWT & Identity Server**
* Containerization using **Docker**
* Kubernetes (K8s) support for orchestration
* Clean Architecture & modular design

---

## 🧩 Microservices Architecture

### 🔐 Identity Service

* Authentication & authorization using **Duende Identity Server**
* ASP.NET Identity integration
* SQL Server database

### 🌐 API Gateway (Web & Admin)

* Centralized routing via **Ocelot**
* JWT-based authentication
* Request aggregation & routing

### 📦 Product Service

* RESTful APIs (CRUD operations)
* JWT authentication
* SQL Server database
* Consumes RabbitMQ events

### 🛒 Basket Service

* Shopping cart management
* **Redis caching** for high performance

### 📉 Discount Service

* High-performance **gRPC service**
* Protobuf-based communication
* SQL Server database

### 📦 Ordering Service

* Order processing workflows
* **MongoDB integration**
* Event-driven communication

### 💳 Payment Service

* Clean Architecture implementation
* Handles payment workflows
* Integrated with event-driven system

---

## 🔗 Communication Patterns

* **Synchronous:** gRPC communication between services
* **Asynchronous:** RabbitMQ (Publish/Subscribe model)

---

## 🐳 Containerization & Deployment

* Dockerized all services and databases
* Managed via **Docker Compose**
* Kubernetes (K8s) deployment support
* Cloud-ready for **Azure Kubernetes Service (AKS)**

---

## ⚙️ Getting Started

### Run using Docker

```bash
docker-compose up --build
```

### Access Services

* API Gateway: http://host.docker.internal:10023
* Product API: http://host.docker.internal:11002/swagger
* Ordering API: http://host.docker.internal:7002/swagger
* Basket API: http://host.docker.internal:6002/swagger
* RabbitMQ Dashboard: http://host.docker.internal:15672 (guest/guest)

---

## 📈 Future Enhancements

* Distributed tracing using **OpenTelemetry & Jaeger**
* Resilience patterns using **Polly (Retry, Circuit Breaker)**
* CI/CD pipelines using **GitHub Actions / Azure DevOps**
* Monitoring using **Prometheus & Grafana**
* Saga pattern for distributed transactions
* Rate limiting and API security improvements

---

## 🙏 Acknowledgment

This project is inspired by open-source microservices architectures and has been extended with custom implementations, enhancements, and modifications for learning and demonstration purposes.

---

## 📌 Summary

This project reflects strong understanding of:

* Microservices architecture
* Distributed systems
* Cloud-native application design
* Backend scalability and resilience patterns

It is designed to simulate real-world enterprise applications and demonstrate production-level backend engineering skills.
