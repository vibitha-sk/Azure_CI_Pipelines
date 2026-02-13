# Azure_CI_Pipelines 🚀

This project demonstrates CI pipeline implementations for [example-voting-app](https://github.com/dockersamples/example-voting-app) by [Docker Samples](https://github.com/dockersamples).The application was imported 
into Azure DevOps where automated pipelines were built for microservices of the application.

### Key Features
- Self-hosted VM agent used to host and run the pipelines.
- Azure Container Registry for storing and managing container images.
- Automated CI pipelines built for each microservice.

### Prerequisites
- A Linux VM with Docker installed and running.
- An Azure Container Registry (ACR) in the same resource group as the VM.
- Integrate the VM with Azure DevOps by adding it as a self-hosted agent in an Agent Pool.

### Setup Architecture & Overview
![Azure CI pipeline architecture1](https://github.com/user-attachments/assets/c941d268-3978-4a4a-aa9e-76c97da3f650)


### Pipeline Structure
The CI pipeline is structured in the following way:

