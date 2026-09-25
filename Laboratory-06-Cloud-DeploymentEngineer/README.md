# Laboratory 06 - Cloud Deployment Engineer

## Mission Overview

In this laboratory activity, I deployed a multi-tier private cloud storage application using Docker Compose. The application consists of a Nextcloud web application and a MariaDB database container. Instead of deploying each container manually, I used a `docker-compose.yml` file to define and deploy the infrastructure as code.

## Objectives

- Explain the roles of different tiers in a multi-container architecture.
- Understand the purpose and structure of a `docker-compose.yml` file.
- Use the Linux command-line text editor `nano` to create configuration files.
- Deploy a multi-container application using Docker Compose.
- Access the Nextcloud web interface through port 8080.
- Document Infrastructure as Code (IaC) concepts using Markdown.

## Commands Executed

```bash
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
docker-compose config
docker-compose up -d
docker-compose ps
docker-compose down

Skills Learned
Creating and editing YAML configuration files using the Linux terminal.
Understanding multi-tier application architecture.
Using Docker Compose to define and manage multiple containers.
Connecting application and database containers using Docker Compose service names.
Using environment variables to configure containerized applications.
Verifying running containers using docker-compose ps.
Deploying and gracefully shutting down a multi-container application.