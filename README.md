# Docker Jenkins CI/CD Pipeline Project

## Overview

This project demonstrates a simple **CI/CD pipeline using Jenkins and Docker**.

The pipeline automatically builds and deploys a Node.js application whenever the code is updated.

---

# Architecture

```text
Developer
   ↓
GitHub Repository
   ↓
Jenkins Pipeline
   ↓
Docker Build
   ↓
Docker Container Deployment
```

---

# Technologies Used

* Docker
* Jenkins
* Node.js
* GitHub

---

# Project Structure

```text
docker-jenkins-cicd
│
├── Dockerfile
├── server.js
├── package.json
└── Jenkinsfile
```

---

# Setup

Clone repository

```
git clone <repo>
cd docker-jenkins-cicd
```

Push code to GitHub.

Configure Jenkins pipeline to use the repository.

Run pipeline to automatically build and deploy the application.

---

# Pipeline Stages

1. Clone repository
2. Build Docker image
3. Remove old container
4. Deploy new container

---

# Access Application

```
http://server-ip:3000
```

---

# DevOps Concepts

* Continuous Integration
* Continuous Deployment
* Docker container deployment
* Jenkins automation pipeline

