# Django eCommerce DevOps Project

A production-grade Django eCommerce application deployed using Docker, GitHub Actions CI/CD pipeline, AWS EC2, Nginx, and Gunicorn.

---

# Project Overview

This project demonstrates a complete DevOps deployment workflow for a Django-based eCommerce application.

The application is containerized using Docker and deployed on an AWS EC2 instance with automated CI/CD using GitHub Actions.

---

# Features

- Django eCommerce Application
- Docker Containerization
- GitHub Actions CI/CD Pipeline
- AWS EC2 Deployment
- Nginx Reverse Proxy
- Gunicorn WSGI Server
- Automated Deployment Workflow
- Linux Server Configuration
- Production Deployment Setup

---

# Tech Stack

| Technology | Purpose |
|---|---|
| Django | Backend Web Framework |
| Docker | Containerization |
| GitHub Actions | CI/CD Automation |
| AWS EC2 | Cloud Hosting |
| Nginx | Reverse Proxy |
| Gunicorn | Application Server |
| Linux | Server Environment |
| Git & GitHub | Version Control |

---

# System Architecture

```text
Developer Pushes Code
        ↓
GitHub Repository
        ↓
GitHub Actions CI/CD
        ↓
Docker Image Build
        ↓
Docker Hub
        ↓
AWS EC2 Server
        ↓
Docker Container
        ↓
Nginx Reverse Proxy
        ↓
Live Django Application
```

---

# Local Setup

## Clone Repository

```bash
git clone https://github.com/YOUR_USERNAME/django-ecommerce-devops.git
```

## Create Virtual Environment

```bash
python -m venv venv
```

## Activate Environment

### Windows

```bash
venv\Scripts\activate
```

### Linux/Mac

```bash
source venv/bin/activate
```

## Install Dependencies

```bash
pip install -r requirements.txt
```

## Run Application

```bash
python manage.py runserver
```

---

# Docker Setup

## Build Docker Image

```bash
docker build -t django-ecommerce-devops .
```

## Run Docker Container

```bash
docker run -p 8000:8000 django-ecommerce-devops
```

---

# CI/CD Pipeline Workflow

1. Developer pushes code to GitHub
2. GitHub Actions pipeline triggers automatically
3. Docker image is built
4. Docker image is pushed to Docker Hub
5. AWS EC2 server pulls latest image
6. Existing container is replaced
7. Updated application goes live

---

# AWS Deployment

The application is deployed on an AWS EC2 Ubuntu instance using Docker containers and Nginx reverse proxy configuration.

---

# Future Enhancements

- HTTPS with SSL
- PostgreSQL Integration
- Kubernetes Deployment
- Terraform Infrastructure Automation
- Monitoring with Prometheus & Grafana

---

# Author

Sushma Janaki
