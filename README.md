# Deploy React App to AWS EC2 Using GitHub Actions 🚀
This repository demonstrates a streamlined CI/CD pipeline to build and deploy a Vite-powered React application to an AWS EC2 instance using GitHub Actions.

## Key Features
- Automated Builds: The React app is automatically built using Docker upon every push to the deploy-to-ec2 branch.
- Containerization: The app is containerized with Docker for consistent deployments.
- Continuous Deployment: GitHub Actions handle the entire deployment process to an EC2 instance.
  
## How It Works
### 1.Build Process:

The React app is built with Vite and Docker on every push.
The Docker image is then published to Docker Hub.

## 2.Deployment Process:

The Docker image is pulled from Docker Hub onto the EC2 instance.
The running container is updated with the latest image.

## Getting Started

### 1.Clone the Repository:

  git clone https://github.com/akithawijesinghe/Deploy-React-app-to-AWS-EC2-GithubAction.git

### 2.Create the deploy-to-ec2 Branch:

  git checkout -b deploy-to-ec2

### 3.Set Up GitHub Actions:

- Update your secrets in GitHub for Docker Hub credentials.
- Push the .github/workflows/cicd.yml file to trigger the workflow.

### 4.Deploy:

- On every push to the deploy-to-ec2 branch, the app will be built, containerized, and deployed to your AWS EC2 instance.

## Prerequisites

- AWS EC2 instance with Docker installed.
- Docker Hub account for storing images.
- GitHub Actions runner configured on the EC2 instance.


