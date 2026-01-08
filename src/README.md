# 🛒 Microservices Demo – Docker & Docker Compose (From Scratch)

This repository documents my **hands-on DevOps learning journey**, where I built and ran a **production-style microservices application locally** using **Docker and Docker Compose**, starting completely from scratch.

---

## 🧠 Project Overview

The application is a **microservices-based e-commerce system** consisting of multiple independent services written in **Go, Node.js, Python, and Java**, all containerized and orchestrated locally.

The focus of this project is **Docker fundamentals, service communication, networking, debugging, and orchestration**, not just running containers.

---

## 🧱 Services in This Project

- **frontend** – Web UI (Go)
- **productcatalogservice** – Product catalog (Go, gRPC)
- **cartservice** – Cart management (Go)
- **currencyservice** – Currency conversion (Node.js, gRPC)
- **paymentservice** – Payment processing (Node.js, gRPC)
- **shippingservice** – Shipping calculation (Go, gRPC)
- **emailservice** – Order confirmation emails (Python)
- **recommendationservice** – Product recommendations (Python)
- **adservice** – Advertisements (Java)
- **redis** – In-memory data store for cart service

All services communicate internally using **Docker DNS and a shared Docker network**.

---

## 🚀 Step-by-Step: What I Did From Scratch

### 1️⃣ Explored the Codebase
- Identified each microservice and its responsibility
- Understood inter-service dependencies
- Reviewed Dockerfiles for different runtimes

### 2️⃣ Built Docker Images for Each Service
Built images manually using Dockerfiles and tags.

### 3️⃣ Ran Services Individually
Used `docker run` to understand ports, logs, and failures.

### 4️⃣ Debugged Real Errors
Fixed missing env vars, port conflicts, profiler issues, and DNS problems.

### 5️⃣ Implemented Docker Networking
Created a custom Docker bridge network for service discovery.

### 6️⃣ Centralized Configuration
Used `.env` files to manage service addresses and configuration.

### 7️⃣ Migrated to Docker Compose
Moved from manual runs to declarative orchestration using Docker Compose.

### 8️⃣ Resolved Conflicts
Handled container name conflicts and clean restarts.

### 9️⃣ Verified Application
Accessed the frontend locally and confirmed inter-service communication.

---

## 🛠 Technologies Used

- Docker
- Docker Compose
- Go, Node.js, Python, Java
- gRPC
- Redis
- Linux
- Bash

---

## 🎯 Key Learnings

- Docker images vs containers
- CMD vs ENTRYPOINT
- Docker networking & DNS
- Environment variables
- Debugging containerized apps
- Production-style orchestration

---

## ▶️ How to Run

```bash
docker compose up -d
```

Open:
http://localhost:8080

---

## 🙌 Author

**Yugandhar Kanaparthi**  
Aspiring DevOps / Cloud Engineer
