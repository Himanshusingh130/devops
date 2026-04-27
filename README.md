# 🚀 INT 396 DevOps Project  
CI/CD-Based Deployment using Docker & GitHub Actions

---

## 📌 Overview
This project demonstrates a complete DevOps pipeline for deploying a Python-based web application. It uses CI/CD automation, Docker containerization, and optional cloud deployment to ensure fast, reliable, and consistent delivery.

---

## 🧱 Tech Stack
- Backend: Flask  
- Containerization: Docker  
- CI/CD: GitHub Actions  
- Version Control: GitHub  
- Deployment: AWS EC2 (optional)

---

## ⚙️ Features
- Automated CI/CD pipeline  
- Docker-based containerized deployment  
- REST API endpoints (`/` and `/health`)  
- Cross-platform compatibility  
- Automated testing using pytest  

---

## 📁 Project Structure
```
int396-devops/
│
├── app.py
├── requirements.txt
├── Dockerfile
├── docker-compose.yml
├── .dockerignore
├── .github/workflows/ci.yml
├── tests/
│   └── test_app.py
└── README.md
```

---

## ▶️ Getting Started

### 1. Clone Repository
```
git clone https://github.com/YOUR_USERNAME/int396-devops.git
cd int396-devops
```

---

### 2. Run Locally
```
pip install -r requirements.txt
python app.py
```

Open in browser:  
http://localhost:5000

---

### 3. Run with Docker
```
docker build -t int396-app .
docker run -p 5000:5000 int396-app
```

---

## 🔁 CI/CD Pipeline
This project uses GitHub Actions for automation.

Pipeline Steps:
1. Code pushed to GitHub  
2. CI/CD pipeline triggered  
3. Dependencies installed  
4. Tests executed  
5. Docker image built  
6. Application ready for deployment  

---

## 🧪 Testing
```
pytest
```

---

## 🌐 API Endpoints

| Endpoint   | Method | Description        |
|------------|--------|--------------------|
| /          | GET    | Home route         |
| /health    | GET    | Health check       |

---

## ☁️ Deployment (AWS EC2 - Optional)
```
docker pull <your-dockerhub-username>/int396-app
docker run -d -p 80:5000 <your-dockerhub-username>/int396-app
```

Access:
```
http://<your-ec2-public-ip>
```

---

## 🏗️ Architecture Flow
Developer → GitHub → GitHub Actions (CI/CD)  
→ Run Tests → Build Docker Image  
→ Deploy to Server → User Access  

---

## 📊 Output
- Web application runs in browser  
- Health endpoint returns JSON status  
- CI/CD pipeline executes automatically  
- Docker ensures consistent environment  

---

## 🧠 Conclusion
This project applies DevOps practices to automate deployment, improve reliability, and ensure scalability.

---

## 📌 Viva One-Liner
This project uses CI/CD and Docker to automate deployment and ensure consistency.

---

## ⚡ Future Enhancements
- Kubernetes deployment  
- Monitoring with Prometheus & Grafana  
- Frontend UI integration  
- ML model integration  

---

## 👨‍💻 Author
Himanshu Singh
