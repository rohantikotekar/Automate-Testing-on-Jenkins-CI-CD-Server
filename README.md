# Automate-Testing-on-Jenkins-CI-CD-Server

## Features

- **Full-Stack Application**: A complete Python-based application with both front-end and back-end components.
- **Dockerized**: The application is containerized using Docker for consistent and scalable deployments.
- **CI/CD Pipeline**: Automated builds and deployments to production with continuous integration and delivery.
- **Automated Testing**: Integration of automated test cases in the CI/CD pipeline to ensure code quality.
- **Multiple Environments**: Deployment across development, testing, and production environments on AWS EC2 servers.

## Prerequisites

- **AWS EC2 Instances**: Three EC2 instances set up for development, testing, and production.
- **Docker**: Docker installed on all servers for containerization.
- **CI/CD Tool**: Jenkins or any CI/CD tool configured for build and deployment automation.
- **GitHub Tokens**: GitHub tokens for repository access and automated builds.

## Setup

1. **Clone the Repository**:
Clone any python full stack web application using: git clone command

## Create a Dockerfile in the root of your project.
Define the necessary instructions to build your application.
Build the Docker image locally and push it to a container registry (e.g., Docker Hub or AWS ECR).
docker build -t your-image-name .
docker tag your-image-name your-registry/your-image-name
docker push your-registry/your-image-name
Set Up EC2 Servers:

## Launch three EC2 instances (dev, test, prod) and configure them with Docker.
 
## Set up a CI/CD pipeline using Jenkins or another tool.
Configure it to build a new Docker image on each commit to the production branch.
Automate deployments to the EC2 instances.
Integrate automated test cases into the CI/CD pipeline to ensure quality before deployment.
Development: Push changes to the dev branch and deploy to the development server.
Testing: Push changes to the test branch and deploy to the testing server.
Production: Push changes to the prod branch to build and deploy to the production server.
Build Failures: Check Docker build logs and ensure that all dependencies are correctly specified.
Deployment Issues: Verify server configurations and ensure that Docker containers are running correctly.
Test Failures: Review CI/CD logs to identify and resolve any issues in automated tests.
Contributions are welcome! Please open issues or submit pull requests. For major changes, open an issue first to discuss the proposed changes.

## License
This project is licensed under the MIT License - see the LICENSE file for details.

Contact
For questions or support, please contact rohantikotekar@gmail.com
