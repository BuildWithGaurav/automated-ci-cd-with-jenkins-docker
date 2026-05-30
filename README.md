# Docker Jenkins CI/CD Pipeline

## Overview

This project demonstrates the implementation of a Continuous Integration and Continuous Deployment (CI/CD) pipeline using Jenkins, Docker, GitHub, and Python.

The pipeline automates the process of building, testing, and deploying a containerized Python application whenever code changes are pushed to the GitHub repository.

## Features

* Automated build process using Jenkins
* Docker containerization
* GitHub integration
* Continuous Integration workflow
* Automated deployment pipeline
* Reproducible application environment

## Tech Stack

* Jenkins
* Docker
* Python
* GitHub
* GitHub Actions

## Project Structure

```text
.
├── .github/
│   └── workflows/
├── Dockerfile
├── Jenkinsfile
├── app.py
├── requirements.txt
└── README.md
```

## CI/CD Workflow

1. Developer pushes code to GitHub.
2. Jenkins detects repository changes.
3. Jenkins pulls the latest source code.
4. Application dependencies are installed.
5. Docker image is built.
6. Container is created and deployed.
7. Deployment status is reported.

## Pipeline Architecture

```text
Developer
    |
    v
 GitHub Repository
    |
    v
 Jenkins Pipeline
    |
    +----> Build Stage
    |
    +----> Test Stage
    |
    +----> Docker Image Build
    |
    +----> Deployment
    |
    v
 Running Container
```

## Docker Build

Build the Docker image:

```bash
docker build -t python-cicd-app .
```

Run the container:

```bash
docker run -p 5000:5000 python-cicd-app
```

## Jenkins Pipeline

The Jenkins pipeline is defined in the Jenkinsfile and automates:

* Source code retrieval
* Build execution
* Docker image creation
* Deployment

## Learning Outcomes

Through this project, I gained practical experience in:

* CI/CD concepts
* Jenkins automation
* Docker containerization
* Pipeline orchestration
* DevOps workflow implementation
* GitHub integration

## Future Improvements

* Add automated testing
* Deploy to AWS EC2
* Push Docker images to Docker Hub
* Add monitoring and logging
* Implement Kubernetes deployment

## Author

Gaurav Singh

B.Tech Computer Science Engineering (Cloud Computing & Virtualization)

AWS Cloud Practitioner | DevOps Enthusiast | Full Stack Developer
