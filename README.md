# Basic CI/CD Pipeline with GitHub Actions and Docker

This repository demonstrates a complete CI/CD pipeline for a simple Node.js application using GitHub Actions and Docker. It is designed to automatically build, test, and deploy the application on every push to the `main` branch.

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


## CI/CD Workflow

The GitHub Actions workflow is triggered on every push to the `main` branch. The steps include:

1. Checkout code from the repository
2. Set up Node.js environment
3. Install dependencies using `npm`
4. Run a basic test script
5. Build a Docker image of the application
6. Push the Docker image to DockerHub

## Secrets Configuration

To enable secure authentication with DockerHub, the following GitHub repository secrets were used:

- `DOCKERHUB_USERNAME` — DockerHub username
- `DOCKERHUB_TOKEN` — DockerHub access token (generated under DockerHub security settings)

