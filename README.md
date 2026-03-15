# Jenkins Docker AWS CI/CD Pipeline
A fully developed CI/CD pipeline using Jenkins that automatically builds, tests, containerises (using Docker), and deploys a Node.js application to AWS.

This project demonstrates a complete CI/CD pipeline using:

- Jenkins
- Docker
- AWS ECR
- AWS EC2
- Node.js

## Architecture

Developer → GitHub → Jenkins → Build → Test → Docker Build → Push to ECR → Deploy to EC2

## Pipeline Stages

1. Checkout code from GitHub
2. Install dependencies
3. Run tests
4. Build Docker image
5. Push image to AWS ECR
6. Deploy container to EC2

## Technologies Used

- Jenkins
- Docker
- AWS ECR
- AWS EC2
- Node.js
- GitHub
