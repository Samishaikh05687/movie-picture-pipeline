# Project Submission Notes

## Movie Picture Pipeline – CI/CD with AWS EKS

### GitHub Repository
GitHub Repository URL:
https://github.com/Samishaikh05687/Movie-Picture-Pipeline

The repository is publicly accessible and contains the complete project source code, infrastructure setup, Kubernetes configuration, and GitHub Actions workflows.

## GitHub Actions Workflows

The project includes the following four CI/CD workflows:

1. Frontend Continuous Integration
2. Backend Continuous Integration
3. Frontend Continuous Deployment
4. Backend Continuous Deployment

Workflow files are located in:

.github/workflows/

- frontend-ci.yaml
- backend-ci.yaml
- frontend-cd.yaml
- backend-cd.yaml

Successful workflow runs can be verified from the GitHub Actions tab of the public repository.

## Application Deployment

The application is deployed on Amazon EKS.

### Frontend Application URL
http:a9138a82c97a04844a52ae63616e8360-166450987.us-east-1.elb.amazonaws.com

### Backend Application URL
http:af682fcbfaafd45d2ba0821f4d91d693-797719528.us-east-1.elb.amazonaws.com

## Infrastructure

The AWS infrastructure was provisioned using Terraform and includes:

- Amazon EKS cluster
- Amazon ECR repositories for frontend and backend container images
- IAM configuration required for CI/CD
- Kubernetes resources used for application deployment

AWS Region: us-east-1

EKS Cluster Name: cluster

## Verification

The following are available in the public GitHub repository and/or submission:

- Complete project source code
- Terraform infrastructure configuration
- Kubernetes deployment and service configuration
- Four GitHub Actions workflows
- Successful CI/CD workflow runs
- Frontend application deployment verification
- Backend application deployment verification
- Kubernetes verification using `kubectl get all`

## Submission Note

This project is submitted with the required public GitHub repository link and application deployment information so that the CI/CD implementation, GitHub Actions workflow runs, and EKS deployment can be reviewed.

Thank you for reviewing my submission.
