
# Crypto CI/CD Pipeline

Overview

This repository contains an automated CI/CD pipeline for a crypto website using Jenkins, SonarQube, Docker, and GitHub Webhooks on AWS. The pipeline ensures continuous integration, code quality checks, and seamless deployment.

# Technologies Used

Jenkins - Automates the CI/CD process

SonarQube - Static code analysis and quality checks

Docker - Containerization for consistent deployments

GitHub Webhooks - Triggers CI/CD pipeline on code changes

AWS - Hosting and infrastructure for the crypto website

# Pipeline Workflow

Code Push: Developer pushes code to GitHub.

Webhook Trigger: GitHub Webhook notifies Jenkins.

Build & Test: Jenkins pulls the code, builds Docker images, and runs tests.

Code Analysis: SonarQube analyzes the code for vulnerabilities and quality issues.

Dockerization: The application is packaged into a Docker container.

Deployment: Docker container is deployed to AWS.

# Prerequisites

AWS account with EC2/ECS/EKS configured

Jenkins server installed and configured

SonarQube set up for code analysis

Docker installed on the Jenkins server

GitHub Webhooks configured

Setup & Installation

# Clone the repository:

git clone https://github.com/mani16003/crypto-ci-cd-pipeline.git
cd crypto-ci-cd-pipeline

Configure Jenkins pipeline with the Jenkinsfile provided.

Set up SonarQube and integrate it with Jenkins.

Configure Docker to build and push images to AWS.

Deploy the containerized application to AWS.

Deployment

The pipeline automatically deploys to AWS upon a successful build.

Can be configured for rolling updates or blue-green deployment.


