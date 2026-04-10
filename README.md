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
<img width="1707" height="758" alt="docker-build" src="https://github.com/user-attachments/assets/583b6ed5-a627-441f-a938-3a5ebec1f93a" />


### Docker Running (Local)
<img width="1709" height="110" alt="docker-ps-local" src="https://github.com/user-attachments/assets/a38e0ed2-415d-481a-9166-a2bbfea9556c" />


### Local Website
<img width="934" height="929" alt="local-site" src="https://github.com/user-attachments/assets/223ab68c-d699-4242-be3a-8ef821306e33" />


### EC2 Instance
<img width="1920" height="833" alt="ec2-instance" src="https://github.com/user-attachments/assets/3a21db7c-9445-42ac-9dc5-741c5a18f226" />


### Docker Running on EC2
<img width="1494" height="338" alt="ec2-docker" src="https://github.com/user-attachments/assets/a04b30e8-be4c-454d-a430-bbe5081f3aaf" />


### Live Website
<img width="1050" height="950" alt="live-site" src="https://github.com/user-attachments/assets/daecabd8-2982-451e-99e3-9fe8ebfdad7b" />


---

## ✅ Outcome
- Successfully containerized a web application using Docker
- Deployed the container on AWS EC2
- Made the application accessible via public IP

---

## 🙌 Conclusion
This project helped in understanding Docker containerization, cloud deployment, and real-world DevOps workflow.
