# Deployment Process Documentation

This document outlines the deployment process for our application.

## Technologies and Tools

- PostgreSQL: Database
- Docker: Containerization
- AWS ECR: Container registry
- AWS CodeBuild: CI/CD pipeline
- AWS EKS: Container orchestration
- AWS CloudWatch: Logging and monitoring

## Deployment Overview

This project has been configured to be automatically deployed when changes is made in the github repo https://github.com/DuytheTeacher/coworking-space-microservices.git thanks to AWS CodeBuild.

You can connect to AWS EKS to specify the running deployment, services and pods.

You can connect to the running application by getting the DNS name from the Loadbalancing in the service. You can you this command `kubectl get service` and look for the EXTERNAL-IP and PORT of coworking service.

Application has been setup Cloudwatch Logging with Container Insight feature which is helpful to monitor and trace.