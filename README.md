# 🚀 Deploying .NET Microservices to Kubernetes and Azure with CI/CD
This project demonstrates how to containerize, deploy, and automate the deployment of .NET microservices using Docker, Kubernetes, Azure Kubernetes Service (AKS), Azure Container Registry (ACR), and CI/CD pipelines with Azure DevOps and GitHub.

It serves as a hands-on guide for building, testing, and deploying multi-container microservice applications from local environments to cloud-native infrastructure, with support for zero-downtime deployments and full CI/CD automation.

## 🧩 Project Structure – Microservices Overview
This solution consists of three core microservices:

### 1. Shopping.Client (MVC Web App)
- ASP.NET MVC application that consumes the Shopping API.
- Initially built as a standalone web app with embedded data.
- Later containerized using Docker and deployed to:
  - Docker Hub
  - Azure Web App for Containers
  - Kubernetes (local & cloud via AKS)

### 2. Shopping.API
- ASP.NET Web API microservice for managing product data.
- Uses MongoDB for data persistence.
- Containerized and deployed via:
  - Docker Compose
  - Azure Container Registry (ACR)
  - Kubernetes (local & cloud)

### 3. MongoDB (NoSQL Database)
- Pulled from the official Docker Hub image.
- Used as a backend database for the Shopping.API service.
- Connected and composed with the API through Docker and Kubernetes.

## ☁️ Cloud-Native & Kubernetes Workflow
This project takes your services through the full cloud-native lifecycle:

✅ Create Dockerfiles for each service

✅ Compose containers locally using Docker Compose

✅ Deploy containers to local Kubernetes cluster

✅ Push Docker images to Azure Container Registry (ACR)

✅ Deploy microservices to Azure Kubernetes Service (AKS)

✅ Enable zero-downtime deployments using Kubernetes features

✅ Automate deployment with CI/CD pipelines via Azure DevOps

## 📦 Tools & Technologies Used
- .NET 8 / ASP.NET Core
- Docker & Docker Compose
- Kubernetes (local and AKS)
- MongoDB
- Azure Container Registry (ACR)
- Azure Kubernetes Service (AKS)
- Azure DevOps Pipelines
- GitHub Actions
