# 🔗 URL Shortener

A backend URL shortening service built with Spring Boot. 
Converts long URLs into short, manageable links and redirects users seamlessly. 
Includes expiration handling and Redis caching for high performance.

## 🚀 Features

- Shortens any valid URL
- Optional expiration time for each shortened URL
- Fast retrieval using Redis caching
- Redirects from short URL to original URL
- API testing enabled via Swagger UI
- Docker support for containerized deployment

## 🧰 Tech Stack
- Java 17
- Spring Boot 3.4.3
- Spring Web, JPA, Validation
- MYSQL
- Redis (caching layer)
- springdoc-openapi (Swagger UI)
- Docker
- Junit & Mockito

## 🐳 Docker Image

You can use the pre-built Docker image directly from Docker Hub:

🔗 [michellec07/spring-boot-url-shortener](https://hub.docker.com/r/michellec07/spring-boot-url-shortener)

## ⚙️ Setup Instruction (Docker Only)

### 📦 Prerequisites

Ensure you have the following installed:

- [Docker](https://docs.docker.com/get-docker/)
- [Docker Compose](https://docs.docker.com/compose/install/)

Clone this repository to get the necessary files:

- `docker-compose.yml` — defines the backend and MySQL containers  

### ▶️ Run the Application

```bash
# Step 1: Pull the pre-built backend image from Docker Hub
docker pull michellec07/spring-boot-url-shortener:latest

# Step 2: Start backend and MySQL containers
docker-compose up -d
```

### 📺 Access the Application

Visit [http://localhost:8080/swagger-ui](http://localhost:8080/swagger-ui) in your browser to access the Swagger UI for testing the API.
