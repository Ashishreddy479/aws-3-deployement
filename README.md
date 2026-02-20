# AWS 3-Tier Deployment (Docker + Jenkins CI/CD)

## 📌 Project Overview
This project demonstrates a simple 3-tier style application deployment using:

- Python (Flask)
- Docker
- Jenkins CI/CD Pipeline
- GitHub

The application is containerized using Docker and automated using a Jenkins pipeline.

---

## 🏗️ Architecture
- Application Layer: Flask App
- Containerization: Docker
- CI/CD Automation: Jenkins
- Version Control: Git & GitHub

---

## 🚀 How to Run Locally

### 1️⃣ Build Docker Image
docker build -t aws-3-tier-app .

### 2️⃣ Run Docker Container
docker run -d -p 5000:5000 aws-3-tier-app

Application runs on:
http://localhost:5000

---

## 🔄 CI/CD Pipeline Stages
- Clone Repository
- Build Docker Image
- Run Docker Container

---

## 🛠️ Tools & Technologies Used
- Python
- Flask
- Docker
- Jenkins
- GitHub
