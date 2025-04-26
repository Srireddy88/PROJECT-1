# PROJECT-1 

# Full-Stack CI/CD Pipeline with GitHub Actions & Docker

## Project Overview

This project demonstrates the implementation of a **full CI/CD pipeline** using **GitHub Actions** to build, test, and deploy a **full-stack application** with **Docker** containers, deployed locally using **Minikube**.

### Features:
- CI/CD pipeline using GitHub Actions
- Backend and Frontend built into Docker images
- Docker images pushed to Docker Hub
- Deployed and tested locally using Minikube

## Technologies Used
- **GitHub Actions** for CI/CD
- **Docker** for containerization
- **Docker Hub** for image storage
- **Minikube** for local Kubernetes deployment
- **Nginx** (for frontend) & **Flask** (for backend)

### Local Setup Instructions

1. **Clone the repository**:

   ```bash
   git clone https://github.com/Srireddy88/PROJECT-1
   cd full-stack-app
   ```

   ## Build Docker images:

### Backend: Build and tag your backend Docker image:

```bash
docker build -t srilakshmiyannam/fullstack-backend:latest ./backend
```
### Frontend: Build and tag your frontend Docker image:

```bash
docker build -t srilakshmiyannam/fullstack-frontend:latest ./frontend
```
### Push Docker images to Docker Hub:

### Push backend image:

```bash
docker push srilakshmiyannam/fullstack-backend:latest
```
### Push frontend image:

```bash
docker push srilakshmiyannam/fullstack-frontend:latest
```
### Deploy to Minikube:
```bash
minikube start
```
## Apply the Kubernetes configurations (using kubectl):
### Open services in Minikube:

```bash
minikube service frontend-service
minikube service backend-service
```
### Note: Ensure Minikube tunnel is running to access services.

### GitHub Actions Workflow
### This project uses GitHub Actions for the CI/CD pipeline:

## Workflow Overview:
### Build:
Docker images for both backend and frontend

### Test:
Running tests (if applicable) after each push to the repository

### Push:
Docker images to Docker Hub

### Deploy:
Deployment is handled locally via Minikube

### Check :
.github/workflows/ci-cd-pipeline.yml file for the complete GitHub Actions setup.

### Deployed Application:

### Frontend:
```bash
http://localhost:30000
```
### Backend:
```bash
http://localhost:30001/api
```
### Github Actions
![Screenshot 2025-04-26 160328](https://github.com/user-attachments/assets/d0455d5b-9b78-4220-ae07-c00ece5e2e5c)
![Screenshot 2025-04-26 175714](https://github.com/user-attachments/assets/bc4b41c3-4d37-41df-93f2-562a0dfb8901)
![Screenshot 2025-04-26 183504](https://github.com/user-attachments/assets/84036904-8bae-4e75-ab33-81625dca8992)
![Screenshot 2025-04-26 182145](https://github.com/user-attachments/assets/a7a3440b-93b8-4b1e-b6e9-5f4d47bd3c14)
![Screenshot 2025-04-26 182217](https://github.com/user-attachments/assets/639652da-cbc3-47e3-aceb-4959f4b784a3)
![Screenshot 2025-04-26 183504](https://github.com/user-attachments/assets/2036a1ce-0bca-4f5d-a8f5-17f21732a338)
when we clicked on Click Here it will open :
![Screenshot 2025-04-26 180914](https://github.com/user-attachments/assets/e4c9ae56-cd3a-4a7a-983e-077142dc4c45)

### With Minikube
![Screenshot 2025-04-26 185334](https://github.com/user-attachments/assets/1e841ff2-8852-4214-b141-22c28c94769f)
![Screenshot 2025-04-26 185359](https://github.com/user-attachments/assets/c080d684-0c3e-490e-ba01-75f33d769dac)
![Screenshot 2025-04-26 185428](https://github.com/user-attachments/assets/9e63dc65-baee-4f78-b9ef-e3396062e925)
![Screenshot 2025-04-26 191636](https://github.com/user-attachments/assets/a7163768-86a1-4e36-bb1d-a85ec0d95192)
![Screenshot 2025-04-26 191651](https://github.com/user-attachments/assets/25388afb-1b99-4fdf-93ea-374e698d68bd)
![Screenshot 2025-04-26 191729](https://github.com/user-attachments/assets/9b11455a-17ad-4338-9aed-45a32b27ec46)
![Screenshot 2025-04-26 190800](https://github.com/user-attachments/assets/46a4cac0-e592-4c85-8412-c7dca899e22d)









