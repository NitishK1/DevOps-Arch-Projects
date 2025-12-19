# DevOps-Arch-Projects

This repository contains curated DevOps architecture and implementation projects
with only essential files for learning and demonstration purposes.

## Projects

### 1. Project2 - PHP Web Application with Jenkins CI/CD
- **Location:** [Project2/](Project2/)
- **Description:** PHP web application with Jenkins pipeline, Docker
  containerization, and Kubernetes deployment
- **Technologies:** PHP, Jenkins, Docker, Kubernetes, Prometheus, Grafana
- **Features:**
  - Jenkins CI/CD pipeline
  - Docker containerization
  - Kubernetes deployment with HPA
  - Monitoring with Prometheus and Grafana

### 2. Project_Azure_DevOps - Azure DevOps Complete Implementation
- **Location:** [Project_Azure_DevOps/](Project_Azure_DevOps/)
- **Description:** Complete Azure DevOps implementation for an Order Management
  System (ProjectX)
- **Technologies:** Azure DevOps, Node.js, Express.js, Azure Web Apps, Bicep
- **Features:**
  - Azure Boards (Epic, User Stories, Tasks)
  - Azure Repos with Git
  - CI/CD Pipelines with staging and production environments
  - Infrastructure as Code with Bicep
  - Automated deployment scripts
  - Manual approval gates for production

## Getting Started

Each project contains its own README with detailed setup instructions,
architecture documentation, and quick-start guides.

### Prerequisites
- Docker (for containerized projects)
- Kubernetes (for K8s deployments)
- Azure CLI (for Azure projects)
- Node.js (for Node.js projects)
- Git

## Project Structure

```
DevOps-Arch-Projects/
├── README.md                    # This file
├── Project2/                    # PHP Web App with Jenkins
│   ├── app/
│   ├── k8s/
│   ├── monitoring/
│   ├── Dockerfile
│   ├── Jenkinsfile
│   └── README.md
└── Project_Azure_DevOps/       # Azure DevOps Implementation
    ├── app/
    ├── config/
    ├── infrastructure/
    ├── pipelines/
    ├── scripts/
    ├── work-items/
    └── README.md
```

## Contributing

These projects are for educational purposes. Feel free to use them as templates
for your own implementations.

## License

Educational/Demo projects - use as needed for learning purposes.
