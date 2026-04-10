# 🚀 Docker Portfolio Deployment on AWS EC2

## 📌 Overview
This project demonstrates containerization using Docker and deployment of a static portfolio website on an AWS EC2 instance.

---

## 🛠️ Tech Stack
- Docker
- AWS EC2
- HTML, CSS
- Linux (Ubuntu)

---

## 📂 Project Files
- index.html
- style.css
- Dockerfile

---

## 🐳 Docker Setup (Local)

### Build Docker Image
docker build -t my-portfolio .

### Run Docker Container
docker run -d -p 8080:80 my-portfolio

### Access Locally
http://localhost:8080

---

## ☁️ AWS EC2 Deployment Steps

1. Launched EC2 instance (Ubuntu)
2. Connected using SSH
3. Installed Docker:
   sudo apt update
   sudo apt install docker.io -y
4. Transferred project using SCP
5. Built Docker image on EC2:
   sudo docker build -t myapp .
6. Ran container:
   sudo docker run -d -p 80:80 myapp

---

## 🌐 Live Demo
http://54.91.161.0

---

## 📸 Screenshots

### Docker Build
![Docker Build](screenshots/docker-build.png)

### Docker Running (Local)
![Docker Local](screenshots/docker-ps-local.png)

### Local Website
![Local Site](screenshots/local-site.png)

### EC2 Instance
![EC2 Instance](screenshots/ec2-instance.png)

### Docker Running on EC2
![EC2 Docker](screenshots/ec2-docker.png)

### Live Website
![Live Site](screenshots/live-site.png)

---

## ✅ Outcome
- Successfully containerized a web application using Docker
- Deployed the container on AWS EC2
- Made the application accessible via public IP

---

## 🙌 Conclusion
This project helped in understanding Docker containerization, cloud deployment, and real-world DevOps workflow.
