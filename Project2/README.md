# Abstergo Corp CI/CD Pipeline - Project 2

## Overview
Complete CI/CD pipeline solution with Docker, Kubernetes, Jenkins, Prometheus, and Grafana monitoring for Abstergo Corp's online shopping portal.

## Architecture
- **CI/CD**: Jenkins pipeline with GitHub integration
- **Containerization**: Docker
- **Orchestration**: Kubernetes with HPA
- **Monitoring**: Prometheus + Grfana

## Reposiory Structure
```
Project2/
├── Dockerfle              # PHP/Apache cationtainer
├── Jenkinsfile            # CI/CD pipeline definition
├── Problem_Statement.txt  # Assignment requirements
├── app/                   # Application code (git submodule)
├── k8s/                   # Kubernetes manifests
│   ├── deployment.yaml
│   ├── service.yaml
│   └── hpa.yaml
└── monitoring/            # Monitoring stck
    ├── promeheus-deployment.yaml
    └── grafana-deployment.yaml
```

## Quck Start

### Prerequisites
- Dcker
- Kuberetes (Docker Desktop or Minikube)Jenkins
- kubectl

### Setup

1. le wih submodules**:
   ```bsh
   gt clo --ecurse-submodules haton
- **Containerittps://github.com/NitishK1/DevOps-Arch-Projects.git
   cd DevOps-Arch-Projects/Project2
   ```

2. **Build Docker image**:
   ```bash
   docker build -t <your-dockerhub-username>/abstergo-website:latest .
   ```

3. **Deploy to Kubernetes**:
   ```bash
   # Update deployment.yaml with your image name
   kubectl apply -f k8s/
   ```

4. **Deploy monitoring**:
   ```bash
   kubectl create namespace monitoring
   kubectl apply -f monitoring/
   ```

### Jenkins Setup

1. **Configure Jenkins**:
   - Install plugins: Docker Pipeline, Kubernetes CLI
   - Add credenials:
     - `dockerhub-credenialtts`: Docker Hub username/password
     - `localkubeconfig`: Kubernetes config file

2. **Create Pipeline**:
   - Point to this repository
   - Jenkins will use the Jenkinsfile

3. **Trigger Build**:
   - Push changes to trigger automatic builds
   - Or manually trigger from Jenkins

## Access

- **Application**: `kubectl port-forwcr deploys containers
- Prometheus monitors the infrastructure
- Grafana visualizes metrics
