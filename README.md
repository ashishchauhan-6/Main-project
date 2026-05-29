# Netflix Ka Bhai

A Netflix-inspired web application built using Flask and deployed with Docker on AWS EC2.

## Features

* Netflix-style user interface
* Flask backend application
* Docker containerization
* Nginx reverse proxy
* Docker Compose deployment
* AWS EC2 hosting
* Kubernetes configuration files

## Technologies Used

* Python
* Flask
* Gunicorn
* Docker
* Docker Compose
* Nginx
* AWS EC2
* Kubernetes

## Architecture

Browser
|
v
Nginx
|
v
Flask Application

## Run Using Docker

docker build -t netflix-app .

docker run -p 5000:5000 netflix-app

## Run Using Docker Compose

docker compose up -d --build

## Project Structure

Main-project/
├── app.py
├── Dockerfile
├── docker-compose.yml
├── nginx/
│   └── default.conf
├── k8s/
│   ├── deployment.yaml
│   ├── service.yaml
│   └── configmap.yaml
└── README.md

## Author

Ashish Chauhan
