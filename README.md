# DevOps Internship Assessment

## 🚀 Objective
Containerize and deploy a Next.js application using Docker, GitHub Actions, and Minikube.

## 🧩 Setup Instructions

### 1️⃣ Local Run
```bash
cd app
npm install
npm run dev
```

### 2️⃣ Build Docker Image
```bash
docker build -t nextjs-devops-app .
docker run -p 3000:3000 nextjs-devops-app
```

### 3️⃣ Minikube Deployment
```bash
minikube start
kubectl apply -f k8s/deployment.yaml
kubectl apply -f k8s/service.yaml
minikube service nextjs-service
```

### 4️⃣ Access App
Visit the Minikube service URL printed in the terminal.

## ⚙️ GitHub Actions
Automates:
- Docker image build on push to `main`
- Push to GitHub Container Registry (GHCR)

## 🧾 Example GHCR Image
```
ghcr.io/SudheerKonduboina/nextjs-devops-app:latest
```

## 🧑‍💻 Author
**Sudheer Konduboina**
