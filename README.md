# local-kubernetes-cluster-with-minikube
Project establishes local Kubernetes cluster with MiniKube and Docker, mirroring cloud environment. Integrates local CI/CD pipelines via GitHub Actions for cost-effective DevOps learning and demonstration in simulated production setup, exploring modern practices and tools.

## Project Structure

- `admin_dashboard/`: Code for the admin dashboard
- `authentication/`: Code for authentication
- `employee_dashboard/`: Code for the employee dashboard
- `static_files/`: Static files
- `deployment.yaml`: Kubernetes deployment configuration
- `Dockerfile`: Docker configuration for containerization
- `manage.py`: Django management script
- `newapp-service.yaml`: Kubernetes service configuration
- `Pipfile`: Python package management file
- `Pipfile.lock`: Locked Python package dependencies
- `requirements.txt`: Python requirements

## Getting Started

### Prerequisites

- [Docker](https://www.docker.com/)
- [MiniKube](https://minikube.sigs.k8s.io/docs/start/)
- [Python 3.10](https://www.python.org/downloads/)
- [pip](https://pip.pypa.io/en/stable/installation/)

### Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/Local-Kubernetes-Cluster-with-MiniKube.git
   cd Local-Kubernetes-Cluster-with-MiniKube

2.**Set up the Python environment**:
    pip install pipenv
    pipenv install
3.**Build the Docker image:**

    docker build -t yourimage:latest .

4.**Start MiniKube:**

    minikube start

5.**Deploy the application to MiniKube:**

  kubectl apply -f deployment.yaml
  kubectl apply -f newapp-service.yaml

6.**Access the application:**

  minikube service newapp-service

## Repo Strucuture for reference 

This structure and information should help you set up your GitHub repository effectively.

Local-Kubernetes-Cluster-with-MiniKube/
├── admin_dashboard/
│ └── (your admin dashboard code)
├── authentication/
│ └── (your authentication code)
├── employee_dashboard/
│ └── (your employee dashboard code)
├── static_files/
│ └── (your static files)
├── deployment.yaml
├── Dockerfile
├── manage.py
├── newapp-service.yaml
├── Pipfile
├── Pipfile.lock
├── requirements.txt
├── README.md
└── .github/
└── workflows/
└── ci-cd-pipeline.yml




