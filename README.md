# AWS 3-Tier Web Application Deployment (Docker + Jenkins CI/CD)

## Overview
This project demonstrates deploying a simple Flask web application using Docker and automating build/deploy using Jenkins CI/CD.

## Tech Stack
- Python (Flask)
- Docker
- Jenkins (CI/CD)
- AWS (concept: 3-tier deployment)

## Files
- app.py - Flask app
- requirements.txt - Dependencies
- Dockerfile - Build container
- Jenkinsfile - CI/CD pipeline
- .gitignore - Ignore files

## Run Locally

```bash
pip install -r requirements.txt
python app.py

## Run with Docker
docker build -t aws-3-deployment .
docker run -p 5000:5000 aws-3-deployment
Open: http://localhost:5000
