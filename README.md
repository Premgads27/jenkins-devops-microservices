# Jenkins DevOps Microservices

A hands-on DevOps project where I built a Jenkins CI/CD pipeline for a Java microservice application.

The goal was to automate the process from **GitHub → Jenkins → Docker → Docker Hub**.

## 🛠️ Tech Stack

* Java / Spring Boot
* Maven
* Jenkins
* Docker
* Docker Compose
* Docker Hub
* Git / GitHub

## 🔄 CI/CD Pipeline

The Jenkins pipeline performs the following steps:

```text
GitHub
   ↓
Jenkins
   ↓
Build & Test
   ↓
Package Application
   ↓
Build Docker Image
   ↓
Push to Docker Hub
```

The pipeline is defined in the `Jenkinsfile`.

## 🐳 Docker

The application is packaged into a Docker image using the `Dockerfile`.

Docker Compose is also included to make running the application locally easier.

## 🚀 Run Locally

Clone the repository:

```bash
git clone https://github.com/Premgads27/jenkins-devops-microservices.git
cd jenkins-devops-microservices
```

Build the application:

```bash
mvn clean package
```

Build the Docker image:

```bash
docker build -t jenkins-devops-microservices .
```

Run it:

```bash
docker run -p 8080:8080 jenkins-devops-microservices
```

Or use Docker Compose:

```bash
docker compose up --build
```

## 📁 Project Structure

```text
jenkins-devops-microservices/
├── src/
├── Dockerfile
├── Jenkinsfile
├── docker-compose.yml
├── pom.xml
└── README.md
```

## 🎯 What I Practised

* Creating a Jenkins pipeline
* Using a `Jenkinsfile`
* Building Java applications with Maven
* Running tests through Jenkins
* Creating Docker images
* Publishing images to Docker Hub
* Connecting GitHub, Jenkins and Docker together

## 👨‍💻 About

This is one of my hands-on projects while building my practical **DevOps and Cloud Engineering** skills.
