# Netflix Ka Bhai

A Netflix-inspired web streaming application built using Flask and deployed on AWS EC2 using Docker, Nginx, and GitHub Actions.

---

## Project Overview

Netflix Ka Bhai is a web application that demonstrates modern DevOps practices including containerization, reverse proxy configuration, CI/CD automation, cloud deployment, and infrastructure management.

The application is containerized using Docker, served through Gunicorn, routed through Nginx, and hosted on an AWS EC2 instance.

---

## Features

* Netflix-inspired user interface
* Flask web application
* Gunicorn production server
* Docker containerization
* Docker Compose orchestration
* Nginx reverse proxy
* GitHub Actions CI/CD pipeline
* Docker Hub image registry
* AWS EC2 deployment
* Automated image build and push

---

## Technology Stack

### Backend

* Python
* Flask
* Gunicorn

### DevOps

* Docker
* Docker Compose
* GitHub Actions
* Docker Hub
* Nginx

### Cloud

* AWS EC2

---

## Architecture

```text
Developer
    |
    v
GitHub Repository
    |
    v
GitHub Actions
    |
    v
Docker Hub
    |
    v
AWS EC2
    |
    v
Docker Compose
    |
    v
Nginx Reverse Proxy
    |
    v
Flask Application (Gunicorn)
```

---

## CI/CD Pipeline

### Continuous Integration (CI)

Whenever code is pushed to the main branch:

1. GitHub Actions starts automatically
2. Project dependencies are installed
3. Tests are executed
4. Docker image is built
5. Docker image is pushed to Docker Hub

### Continuous Delivery (CD)

Deployment-ready Docker images are automatically available in Docker Hub and can be deployed to AWS EC2.

---

## Project Structure

```text
Main-project/
│
├── app.py
├── requirements.txt
├── Dockerfile
├── docker-compose.yml
│
├── nginx/
│   └── default.conf
│
├── .github/
│   └── workflows/
│       ├── ci.yml
│       └── ci-cd.yaml
│
├── static/
├── templates/
│
└── README.md
```

---

## Run Locally

### Clone Repository

```bash
git clone <repository-url>
cd Main-project
```

### Build Docker Image

```bash
docker build -t netflix-ka-bhai .
```

### Run Container

```bash
docker run -d -p 5000:5000 netflix-ka-bhai
```

Open:

```text
http://localhost:5000
```

---

## Run Using Docker Compose

```bash
docker compose up -d --build
```

Check containers:

```bash
docker compose ps
```

View logs:

```bash
docker compose logs
```

---

## Docker Hub

Docker images are automatically built and pushed using GitHub Actions.

Image Tags:

* latest
* commit SHA tags

---

## AWS Deployment

The application is deployed on an AWS EC2 Ubuntu instance.

Services running on EC2:

* Docker Engine
* Docker Compose
* Nginx Reverse Proxy
* Flask Application

---

## Learning Outcomes

This project helped in understanding:

* Linux Administration
* AWS EC2
* Docker
* Docker Compose
* Nginx
* GitHub Actions
* CI/CD Pipelines
* Docker Hub
* Cloud Deployment

---

## Future Improvements

* Automatic EC2 deployment using GitHub Actions
* Health checks and monitoring
* HTTPS using SSL certificates
* Custom domain integration
* Application scaling

---

## Author

Ashish Chauhan

