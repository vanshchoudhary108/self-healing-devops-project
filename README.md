# 🚀 Self-Healing Container Deployment & Monitoring

## 📌 Project Overview
This project demonstrates a self-healing containerized application deployed on Kubernetes. It also includes automation using Ansible and a CI/CD pipeline using Jenkins.

---

## 🛠️ Tools & Technologies
- Docker
- Kubernetes (Minikube)
- Jenkins
- Ansible
- Git & GitHub

---

## ⚙️ Features
- Containerized application using Docker
- Deployment on Kubernetes cluster
- Self-healing using Kubernetes Deployment (auto pod restart)
- Automated deployment using Ansible
- CI/CD pipeline using Jenkins

---

## 📂 Project Structure
self-healing-devops-project/
│
├── app/
├── docker/
├── k8s/
├── ansible/
├── Jenkinsfile
└── README.md

---

## 🚀 How to Run
### 1. Start Minikube
```bash
minikube start
```

### 2. Build Docker Image
```bash
eval $(minikube docker-env)
docker build -t self-healing-app -f docker/Dockerfile .
```

### 3. Deploy to Kubernetes
```bash
kubectl apply -f k8s/
```

### 4. Access Application
```bash
minikube service my-service
```

### 5. Self-Healing Demo
```bash
kubectl delete pod <pod-name>
```

## 💡 Note
> This project demonstrates a complete DevOps workflow from containerization to deployment and automation.
