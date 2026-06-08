# CI/CD Pipeline Automation on AWS EKS

## Project Overview

Implemented an end-to-end CI/CD pipeline using GitHub, Jenkins, Maven, Docker, Kubernetes (Amazon EKS), and AWS Elastic Load Balancer.

The pipeline automatically:

* Pulls source code from GitHub
* Builds the application using Maven
* Creates a Docker image
* Pushes the image to Docker Hub
* Deploys the application to Amazon EKS
* Exposes the application using AWS Load Balancer

## Tech Stack

* Git & GitHub
* Jenkins
* Maven
* Docker
* Kubernetes
* Amazon EKS
* AWS ELB
* Linux

## Architecture

GitHub → Jenkins → Maven Build → Docker Build → Docker Hub → Amazon EKS → Load Balancer

## Key Learnings

* CI/CD pipeline automation
* Containerization using Docker
* Kubernetes deployments and services
* EKS cluster management
* Troubleshooting pod scheduling issues
* Load Balancer configuration

## Application URL

Deployed application:

/maven-web-app

Challenges Faced

- Pods remained in Pending state due to EKS node capacity limits.
- Diagnosed issue using kubectl get events.
- Identified "Too many pods" scheduling error.
- Recreated worker node group with larger capacity.
- Verified pod health and LoadBalancer connectivity.

Note: The application was deployed on AWS Free Tier for demonstration purposes.
Infrastructure has been decommissioned to avoid ongoing cloud charges.
Deployment screenshots and architecture diagrams are included below.



