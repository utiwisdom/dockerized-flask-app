# 🐳 Dockerized Flask Application

![Docker](https://img.shields.io/badge/Container-Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Python](https://img.shields.io/badge/Language-Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Framework-Flask-000000?style=for-the-badge&logo=flask&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

---

# 📌 Project Overview

This project demonstrates how to containerize a simple Python Flask application using Docker.

The goal was to understand how Docker creates consistent, portable environments that simplify application deployment across development and production systems.

---

# 🚀 What I Built

- A simple Flask web application
- A custom Docker image using a Dockerfile
- A fully isolated containerized environment
- Port mapping between host and container
- Reproducible deployment workflow

---

# 🖼️ Application Running Successfully

![Docker App Running](screenshots/browser-output.png)

---

# 🧠 Key Concepts Learned

| Concept | Explanation |
|---|---|
| Docker Images | Blueprint used to create containers |
| Containers | Lightweight isolated runtime environments |
| Dockerfile | Instructions for building Docker images |
| Port Mapping | Allows browser access to containerized apps |
| Environment Consistency | Eliminates “works on my machine” issues |

---

# 🔍 Dockerfile Breakdown

```dockerfile
FROM python:3.9

WORKDIR /app

COPY . .

RUN pip install flask

CMD ["python", "app.py"]
```

---

# 💭 My Reflection

### Why is Docker important?

Docker simplifies deployment by packaging the application, dependencies, and runtime environment into a portable container.

### What problem does Docker solve?

It prevents dependency conflicts and ensures applications behave consistently across different machines and environments.

### Business Impact

- Faster developer onboarding
- Reduced deployment failures
- Improved scalability
- More reliable CI/CD workflows

---

# ▶️ How to Run the Project

## Build Docker Image

```bash
docker build -t flask-app .
```

## Run Container

```bash
docker run -p 5000:5000 flask-app
```

---

# 🌐 Access the Application

```text
http://localhost:5000
```

Expected Output:

```text
Hello, Docker!
```

---

# 📚 Technologies Used

- Python
- Flask
- Docker

---

# 🚀 Future Improvements

- Add Docker Compose
- Connect PostgreSQL database
- Deploy to cloud
- Add CI/CD pipeline
- Convert into microservice architecture
