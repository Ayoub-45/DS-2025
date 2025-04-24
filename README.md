# DS-2025 CI/CD Pipeline with GitHub Actions

This repository contains a CI/CD pipeline that automatically builds and publishes a Docker image for a Python application using **GitHub Actions** and the **GitHub Container Registry (GHCR)**.

## 🚀 Objectives Achieved

- ✅ Forked and cloned the `DS-2025` repository from [nawelbay/DS-2025](https://github.com/nawelbay/DS-2025)
- ✅ Created a GitHub Actions workflow named `DSPipeline`
- ✅ Built a Docker image named `mydsapp` for the Python application
- ✅ Published the Docker image to GitHub Container Registry at:

## 🔧 CI/CD Workflow Details

- **Workflow File:** `.github/workflows/DsPipeline.yaml`
- **Workflow Name:** `DSPipeline`
- **Triggered On:** Push and Pull Request to `main` branch
- **Job Name:** `DockerBuildPublish`
- **Build Environment:** `ubuntu-latest`
- **Registry:** GitHub Container Registry (GHCR)
- **Authentication:** Uses `GITHUB_TOKEN` for secure Docker login

## 🐳 Docker Image

The Docker image is built from the root of the project and tagged as:


Replace `<your-username>` with your GitHub username when pulling the image.

## 📦 How to Pull the Image

```bash
docker pull ghcr.io/<your-username>/mydsapp:latest

.github/
└── workflows/
    └── DsPipeline.yaml
Dockerfile
README.md
