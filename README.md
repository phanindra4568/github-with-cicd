🚀 Python CI/CD Pipeline with Docker & GitHub Actions (Local Deployment)

This project demonstrates a complete CI/CD pipeline using GitHub Actions, Docker, and Minikube to build, test, and deploy a simple Python Flask application.

🧰 Tools Used

🐍 Python + Flask

🐳 Docker

📦 Docker Hub

⚙️ GitHub Actions

☸️ Minikube / Local Kubernetes

📁 Project Structure

project-root/

├── app/

│ ├── main.py # Flask application

│ └── test_main.py # Unit tests using Pytest

├── Dockerfile # Docker build instructions

├── requirements.txt # Python dependencies

├── docker-compose.yml # Optional: Local Docker run

└── .github/

└── workflows/

    └── ci-cd.yml      # GitHub Actions workflow
🔄 CI/CD Workflow

Trigger:

Runs on every push to the main branch.

Workflow Actions:

✅ Checkout the source code

🧪 Run unit tests using pytest

🛠️ Build the Docker image

📤 Push the image to Docker Hub

Repository: ravindranadratagore/cicd

🔐 GitHub Secrets Required

Name Description

DOCKER_USERNAME Docker Hub username

DOCKER_PASSWORD Docker Hub password or token

🧪 Build & Run Locally

Using Docker Compose (optional):

docker-compose up --build

Run Docker manually:

docker run -d -p 3000:5000 ravindranadhtagore/ci-cd:latest

☸️ Deploy on Minikube

minikube start --driver=docker

kubectl create deployment myapp --image=phanindra4568/ci-cd:latest

kubectl expose deployment myapp --type=NodePort --port=5000

minikube service myapp

📦 Deliverables

GitHub Repository:

https://github.com/phanindra4568/github-with-cicd.git

Docker Image:

https://hub.docker.com/repository/docker/phanindra4568/ci-cd/general

CI/CD Logs:

GitHub Actions Tab

https://github.com/phanindra4568/github-with-cicd/actions

Deployed App (Demo URL):

http://43.205.119.116:3000/

Deployment Screenshot:

![image](https://github.com/user-attachments/assets/c0a0f6e7-2b93-4dd4-9f28-abf30b88738d)

