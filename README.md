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
<img width="911" height="511" alt="new ci arch drawio" src="https://github.com/user-attachments/assets/eba33274-db36-43e1-ac15-6009652cc66f" />


### How it works
- **Import Source Code** — The example-voting-app source code is imported 
   from GitHub into Azure DevOps as the base for the CI pipeline.
- **Configure Self-hosted Agent** — A Linux VM with Docker installed is 
   integrated with Azure DevOps by registering it as a self-hosted agent 
   in an Agent Pool.
-  **Implement CI Pipelines** — Dedicated CI pipelines are created for each 
   microservice — Vote, Worker and Result — using YAML pipeline definitions.
- **Trigger Pipelines** — Pipelines are automatically triggered on every 
   code change pushed to the repository.
- **Build and Push Images** — The self-hosted VM agent builds Docker images 
   for each microservice and pushes them to Azure Container Registry (ACR).

### Pipeline Demonstrations
<img width="2100" height="717" alt="Screenshot 2026-02-12 152538" src="https://github.com/user-attachments/assets/30ca65f7-8dda-4b95-81a0-8e66526c629a" />
<img width="2169" height="661" alt="Screenshot 2026-02-12 153554" src="https://github.com/user-attachments/assets/205bee59-6a7f-4d96-a3a0-4a639cb35fdd" />




