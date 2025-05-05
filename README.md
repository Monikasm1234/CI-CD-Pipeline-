# CI/CD Pipeline with GitHub Actions and Docker

## Overview
This project demonstrates a CI/CD pipeline that:
- Builds a Docker image from a Flask app.
- Pushes it to Docker Hub using GitHub Actions.
- Deploys the image on a local Minikube Kubernetes cluster.

## Prerequisites
- Docker Desktop
- Minikube
- kubectl CLI
- GitHub Account & Docker Hub Account

## Usage
1. Clone the repository.
2. Add GitHub secrets: `DOCKER_USERNAME`, `DOCKER_PASSWORD`.
3. Push to main branch to trigger CI/CD pipeline.
4. Deploy locally:
```bash
minikube start
kubectl apply -f deployment.yaml
minikube service ci-cd-service
```

## Author
Demo Project for CI/CD with Docker and GitHub Actions
