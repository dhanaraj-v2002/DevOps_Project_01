# DevOps Application Deployment

## 📌 Project Overview
This project demonstrates deploying a React application using Docker, AWS ECR, AWS EKS, and CI/CD pipeline with CodeBuild and CodePipeline.

---

## 🚀 Steps Implemented

### 1. Application Setup
- Cloned GitHub repository
- Application runs on port 3000

---

### 2. Docker
- Created Dockerfile
- Built Docker image
- Verified container output

---

### 3. AWS ECR
- Created repository
- Pushed Docker image to ECR

---

### 4. Kubernetes (EKS)
- Created EKS cluster
- Created deployment.yaml and service.yaml
- Deployed application using kubectl

---

### 5. CodeBuild
- Created build project
- Connected GitHub repository
- Defined build commands in buildspec.yml

---

### 6. CodePipeline
- Source: GitHub
- Build: CodeBuild
- Deploy: EKS via kubectl (automated)

---

### 7. Monitoring
- Used CloudWatch logs to track build and deployment

---

## 🔄 CI/CD Workflow

Code Push → CodePipeline → CodeBuild → Docker Build → ECR → kubectl deploy → EKS

---

## 🌐 Application Access

LoadBalancer URL: http://a7f947bf6ca3b474ca8fe183a97fe196-1196077578.ap-south-1.elb.amazonaws.com/
