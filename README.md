# Node.js CI/CD Pipeline with GitHub Actions and Docker

This repository demonstrates how to automate the deployment of a sample Node.js web application using GitHub Actions and Docker.

--------------------------------------------------------------------------------------------------------------------------------

## 🚀 Objective

Set up a complete CI/CD pipeline to:
- Automatically test
- Build a Docker image
- Push it to Docker Hub

All triggered on every `push` to the `main` branch.

---------------------------------------------------------------------------------------------------------------------------------

## 🛠️ Tools & Technologies Used

- Node.js
- GitHub Actions
- Docker & Docker Hub
- GitHub Secrets

---

## 📁 Project Structure

├──.gitignore

├── .github/workflows/main.yml   # GitHub Actions CI/CD pipeline

├── Dockerfile   # Docker image configuration

├── index.js     # Main Node.js app file

├── package.json # Node.js dependencies and metadata

├── README.md    # Project overview


## ⚙️ GitHub Actions Workflow
The pipeline is defined in `.github/workflows/main.yml` and includes the following steps:

1. **Checkout code**
2. **Set up Node.js**
3. **Install dependencies**
4. **Run tests (optional)**
5. **Build Docker image**
6. **Log in to Docker Hub**
7. **Push image to Docker Hub**

--------------------------------------------------------------------------------------------------------------------------

## 🔐 Required GitHub Secrets

Go to **Settings → Secrets → Actions** and add the following:

| Name               | Description                      |
|--------------------|----------------------------------|
| `DOCKER_USERNAME`  | Your Docker Hub username         |
| `DOCKER_PASSWORD`  | Your Docker Hub password or PAT  |

---

## 📦 DockerHub

The image is pushed to DockerHub under the format:

docker.io/your-dockerhub-username/image-name:latest

---------------------------------------------------------------------------------------------------------------------------

## 📌 How to Use This Repo

1. Fork or clone the repo.
2. Add your Docker Hub credentials as GitHub secrets.
3. Push code to `main` branch.
4. GitHub Actions will automatically build and push the Docker image.

----------------------------------------------------------------------------------------------------------------------------

## 🙌 Author

**Gourav Sharma** 
