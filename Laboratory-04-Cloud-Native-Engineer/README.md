# Laboratory 04 – Cloud-Native Engineer

## Mission Overview

This laboratory activity focused on understanding cloud-native technologies, particularly the difference between Virtual Machines (VMs) and Containers. I used a Docker environment to pull and run an Nginx web server, verify that it was working, and manage the container through different lifecycle commands. The activity also helped me practice documenting technical procedures using Markdown and maintaining my Cloud Computing GitHub portfolio.

## Objectives

* Differentiate between traditional Virtual Machines and Containers.
* Access and use a Docker-enabled cloud environment.
* Execute fundamental Docker CLI commands.
* Pull and run an Nginx containerized web server.
* Manage and terminate a Docker container.
* Document container operations using Markdown.
* Continue developing an organized GitHub Cloud Computing Portfolio.

## Docker Commands Executed

### Checkpoint 3 – Enter the Docker Playground

```bash
docker --version
docker info
```

### Checkpoint 4 – Deploy Your First Container

```bash
docker pull nginx
docker run -d -p 8080:80 nginx
curl http://localhost:8080
```

### Checkpoint 5 – The Container Lifecycle

```bash
docker ps
docker stop <container_id>
docker ps -a
docker rm <container_id>
```

> **Note:** Replace `<container_id>` with the actual container ID shown in your terminal.

## Skills Learned

* Learned how to use basic Docker CLI commands.
* Learned how to pull Docker images from Docker Hub.
* Learned how to run and manage containers.
* Learned how to map ports for a containerized web server.
* Learned how to verify whether an Nginx web server is running.
* Learned how to stop and remove Docker containers.
* Improved my Markdown documentation and GitHub portfolio organization.

## Challenges Encountered

One challenge I encountered was becoming familiar with the different Docker commands and their purposes. I also needed to carefully check the container status when stopping and removing the Nginx container. Another challenge was making sure that the port mapping was correct so that the Nginx web server could be accessed through `localhost:8080`. By following the commands step by step and checking the terminal output, I was able to complete the required Docker tasks successfully.
