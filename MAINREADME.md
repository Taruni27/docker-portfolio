# Dockerized Portfolio Deployment on AWS EC2 (CI/CD with GitHub Actions)

## Project Overview
This project demonstrates a complete CI/CD pipeline to deploy a Dockerized portfolio website on AWS EC2 using GitHub Actions.

The pipeline automates deployment from code push to live website.

---

## Architecture

Developer (Local Machine)
        |
        | git push
        v
GitHub Repository
        |
        | GitHub Actions (CI/CD)
        v
AWS EC2 Instance (Ubuntu)
        |
        | Docker
        v
Nginx Container
        |
        v
Live Website (Public IP)

---

## Tech Stack
- AWS EC2 (Ubuntu)
- Docker
- Nginx
- GitHub Actions
- Git & GitHub
- SSH Key Authentication

---

## Deployment Flow

### 1. Development
Create portfolio files:
- index.html
- style.css
- script.js
- Dockerfile

---

### 2. Push to GitHub
git add .
git commit -m "deploy project"
git push origin main

---

### 3. CI/CD Pipeline (GitHub Actions)
- Clone repository
- Connect to EC2 via SSH
- Trigger deployment script

---

### 4. EC2 Deployment
git pull origin main
docker stop myapp || true
docker rm myapp || true
docker build -t myapp .
docker run -d -p 80:80 --name myapp myapp

---

## Docker Role
- Containerizes application
- Ensures consistent environment
- Runs Nginx web server
- Serves static website

---

## Nginx Role
- Acts as web server
- Serves HTML/CSS/JS files
- Handles HTTP requests
- Runs inside Docker container

---

## CI/CD Architecture

Continuous Integration:
- Code pushed to GitHub
- GitHub Actions triggered

Continuous Deployment:
- EC2 server pulls code
- Docker rebuilds container
- New version deployed automatically

---

## Security
- SSH key-based authentication
- Secrets stored in GitHub (HOST, USERNAME, SSH_KEY)

---

## Final Output
http://<EC2-PUBLIC-IP>

Example:
http://23.20.225.147

---

## Key Learnings
- CI/CD pipelines using GitHub Actions
- Docker containerization
- AWS EC2 deployment
- Nginx web hosting
- Secure SSH deployment

---

## Future Improvements
- Add custom domain
- Enable HTTPS (Let’s Encrypt)
- Docker Hub integration
- Monitoring & logging
