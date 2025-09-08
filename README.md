# Flask CI/CD Demo

A containerized Flask application with automated CI/CD pipeline demonstrating DevOps practices learned during my internship.

## Overview

This project implements a complete CI/CD workflow using GitHub Actions to automatically build and deploy a Docker image to GitHub Container Registry. The pipeline triggers on every push to the main branch, ensuring consistent and reliable deployments.

## Technical Implementation

**Application Stack:**
- Python Flask web application
- Docker containerization
- GitHub Container Registry (GHCR)

**CI/CD Pipeline:**
- GitHub Actions workflow automation
- Automated Docker image building and pushing
- Dynamic tagging based on Git metadata
- Secure authentication using GitHub tokens

## Workflow Features

- **Automatic triggering** on push to main branch
- **Metadata extraction** for consistent image tagging
- **Secure authentication** using GitHub's native token system
- **Multi-stage workflow** for automated deployment

## Usage

Pull and run the latest image:
```bash
docker pull ghcr.io/k0ws03/flask-cicd-demo:main
docker run -p 5000:5000 ghcr.io/k0ws03/flask-cicd-demo:main
```