# Basic CI/CD Pipeline with GitHub Actions and Docker

This project demonstrates a basic CI/CD pipeline using **GitHub Actions** to build and push a Dockerized Node.js app to **Docker Hub**.


## Overview

The project includes:

- A sample Node.js application using Express
- CI/CD automation using GitHub Actions
- Docker image build and deployment to DockerHub

## Tech Stack

- Node.js
- Express.js
- GitHub Actions
- Docker
- DockerHub

## Project Structure

basic-ci-cd/
├── .github/workflows/main.yml # CI/CD workflow definition

├── Dockerfile # Docker image build configuration

├── index.js # Entry point of the Node.js app

├── package.json # Project metadata and dependencies

└── README.md # Project documentation



##  GitHub Actions Workflow

The GitHub Actions pipeline:

1. Checks out the code.
2. Logs into Docker Hub using secrets.
3. Builds the Docker image.
4. Pushes the image to your Docker Hub account.

###  Secrets Required

Make sure to add these secrets to your GitHub repository:
- `DOCKER_USERNAME`
- `DOCKER_TOKEN` (Personal Access Token from Docker Hub)

##  Docker Image

The image is automatically pushed to Docker Hub after every push to `main`.

➡️ [View on Docker Hub](https://hub.docker.com/repository/docker/ayush497/basic-ci-cd)

