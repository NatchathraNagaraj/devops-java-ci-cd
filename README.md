# 🚀 End-to-End DevOps CI/CD Pipeline for Spring Boot

## 📌 Overview
This project demonstrates a **production-style DevOps CI/CD pipeline** for a Java Spring Boot application.  
It covers the complete DevOps lifecycle including **CI automation, containerization, reverse proxying, monitoring, alerting, and API documentation** using industry-standard tools.

---

## 🧰 Tech Stack
- Java 17, Spring Boot
- GitHub Actions (CI)
- Docker & Docker Compose
- NGINX (Reverse Proxy)
- Prometheus (Monitoring)
- Grafana (Dashboards & Alerts)
- Swagger / OpenAPI (API UI)
- WSL (Ubuntu)

---

## 🏗️ Architecture
Client
↓
NGINX
↓
Spring Boot Application
↘
Prometheus → Grafana

yaml
Copy code

---

## ✨ Key Features
- Automated CI pipeline with GitHub Actions
- Dockerized Spring Boot backend
- Multi-container setup using Docker Compose
- NGINX reverse proxy in front of backend service
- Application health and metrics via Spring Boot Actuator
- Metrics collection using Prometheus
- Monitoring dashboards and alerts using Grafana
- Interactive API documentation using Swagger UI

---

## ▶️ Run Locally

### Prerequisites
- Docker
- Docker Compose
- Git

### Steps
```bash
git clone https://github.com/NatchathraNagaraj/devops-java-ci-cd.git
cd devops-java-ci-cd/healthapp
docker-compose up -d --build
🌐 Service URLs
Service	URL
Health Check	http://localhost/actuator/health
Sample API	http://localhost/hello
Swagger UI	http://localhost/swagger-ui.html
Prometheus	http://localhost:9090
Grafana	http://localhost:3000

Grafana Login

Username: admin

Password: admin

📊 Monitoring & Alerting
JVM Heap and Non-Heap memory metrics

HTTP request monitoring

Prometheus used for metrics scraping

Grafana dashboards for visualization

Alert configured for high JVM heap usage

🧪 Sample API
http
Copy code
GET /hello
Response:

text
Copy code
Hello from DevOps CI/CD Project 🚀
📄 CI/CD Pipeline
Triggered on push to main

Maven build for Spring Boot application

Docker image build and validation

CI health verification via GitHub Actions

🧠 What This Project Demonstrates
End-to-end CI/CD implementation

Containerized backend architecture

Reverse proxy configuration using NGINX

Monitoring and alerting using Prometheus & Grafana

Debugging real-world CI/CD and container issues

Secure GitHub authentication using Personal Access Tokens
