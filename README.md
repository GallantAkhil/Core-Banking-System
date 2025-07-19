# 🏦 Core Banking System – Microservices Architecture

> 🚀 A production-grade **Core Banking System (CBS)** built with **Spring Boot Microservices**, featuring secure user authentication, account and transaction management, loan handling, and admin operations. Fully containerized and deployable on **Google Cloud Platform (GCP)** using Docker and Kubernetes.

---

## 📦 Microservices Overview

| Service              | Description                                              |
|----------------------|----------------------------------------------------------|
| `auth-service`       | JWT-based login, registration, and role-based auth       |
| `user-service`       | Profile & KYC management, role assignments               |
| `account-service`    | Create, freeze, close, and view bank accounts            |
| `transaction-service`| Deposits, withdrawals, transfers, and transaction logs   |
| `loan-service`       | Loan application, status tracking, EMI schedule          |
| `biller-service`     | Add/view billers, simulate bill payments                 |
| `notification-service`| Send mock email/SMS alerts                              |
| `admin-service`      | Admin dashboard for user/account oversight               |
| `gateway-service`    | Central API gateway (Spring Cloud Gateway)               |
| `discovery-service`  | Service registry (Eureka)                                |
| `config-service`     | Centralized configuration using Spring Cloud Config      |

---

## 🔐 Key Features

- ✅ JWT-based Authentication & RBAC
- ✅ Isolated PostgreSQL DB per service
- ✅ API Gateway with Route Management
- ✅ Spring Cloud Config for centralized properties
- ✅ Dockerized with `docker-compose`
- ✅ GCP-ready (GKE + Cloud SQL + Load Balancer)
- ✅ OpenAPI documentation per service
- ✅ Easily extensible for frontend & mobile clients

---

## ☁️ Cloud Deployment (GCP)

| Component        | GCP Service              |
|------------------|--------------------------|
| Hosting          | GKE (Google Kubernetes Engine) |
| Databases        | Cloud SQL (PostgreSQL)   |
| Secrets          | Secret Manager           |
| Storage          | Cloud Storage (e.g., for docs) |
| Monitoring       | Cloud Monitoring + Logging |
| CI/CD            | GitHub Actions / Cloud Build |

---

## 🧰 Tech Stack

- **Java 17**, **Spring Boot 3**
- **Spring Security**, **Spring Cloud Gateway**
- **Eureka**, **Spring Cloud Config**
- **PostgreSQL**, **JPA/Hibernate**
- **Docker**, **Docker Compose**
- **Swagger/OpenAPI**, **Lombok**
- *(Optional)* RabbitMQ / Kafka for async events

---

## 🚀 Getting Started (Local)

### 1. Clone the Repo
```bash
git clone https://github.com/your-username/core-banking-system-microservices.git
cd core-banking-system-microservices
