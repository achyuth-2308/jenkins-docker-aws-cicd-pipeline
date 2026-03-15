# Jenkins Docker AWS CI/CD Pipeline

This project demonstrates a complete CI/CD pipeline that automatically builds, tests, containerizes, and deploys a Node.js application using Jenkins.

## Technologies Used

- Jenkins
- Docker
- AWS ECR
- AWS EC2
- Node.js
- GitHub

## Architecture

Developer → GitHub → Jenkins → Build → Test → Docker Build → Push Image to AWS ECR → Deploy Container to EC2

## Project Structure

jenkins-docker-aws-cicd-pipeline

app.js – Node.js application  
test.js – Test file  
package.json – Project dependencies  
Dockerfile – Docker image configuration  
Jenkinsfile – Jenkins pipeline configuration  
deploy_remote.sh – Deployment script for EC2  

## Jenkins Pipeline Stages

1. Checkout code from GitHub
2. Install Node dependencies
3. Run automated tests
4. Build Docker image
5. Push image to AWS ECR
6. Deploy container on AWS EC2

## How the Pipeline Works

1. A developer pushes code to GitHub.
2. Jenkins is triggered through a webhook.
3. Jenkins pulls the latest code.
4. Dependencies are installed and tests are executed.
5. Docker builds an image for the application.
6. The image is pushed to AWS ECR.
7. The EC2 server pulls the new image and runs the container.
