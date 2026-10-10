# Laboratory 07 - Cloud Operations Engineer

## Mission Overview

The mission of this laboratory is to monitor the health and performance of a server and its Docker container. It involves checking system resources, deploying an Nginx container, analyzing application logs, and observing real-time container metrics.

## Objectives

- Check the server's RAM usage and available disk storage.
- Monitor CPU load and running processes.
- Deploy an Nginx container named `client-website`.
- Generate successful HTTP requests and simulate a 404 error.
- Retrieve and analyze application logs using Docker.
- Monitor container CPU and memory consumption using Docker Stats.
- Document the results of the monitoring activities.

## Monitoring Commands Executed

| Command | Purpose |
|---|---|
| `free -h` | Checks the server's memory usage. |
| `df -h /` | Checks the available disk storage of the root filesystem. |
| `top` | Displays running processes, CPU usage, and system load. |
| `docker run -d -p 8080:80 --name client-website nginx` | Creates and starts the Nginx container with port 8080 mapped to port 80. |
| `curl http://localhost:8080` | Sends an HTTP request to test the Nginx website. |
| `curl http://localhost:8080/hidden-admin-page` | Simulates a request to a nonexistent page to generate an HTTP 404 response. |
| `docker logs client-website` | Displays the container's logs, including HTTP requests and errors. |
| `docker stats` | Monitors the container's real-time CPU, memory, network, and block I/O usage. |

## Skills Learned

- Monitoring server memory, disk storage, CPU usage, and running processes.
- Deploying and testing an Nginx Docker container.
- Using `curl` to send HTTP requests and identify successful and failed responses.
- Reading application logs to troubleshoot errors.
- Monitoring container resource consumption using Docker Stats.
- Recording technical findings and organizing screenshots for documentation.