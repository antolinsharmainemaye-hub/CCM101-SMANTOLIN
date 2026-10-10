# Mission Reflection

This laboratory helped me understand the importance of monitoring servers and Docker containers in a Linux environment. I learned that checking resources, analyzing logs, and monitoring container performance are important tasks for a Cloud Operations Engineer.

First, checking the host server's resources is important even if the containers are running perfectly because containers still depend on the host's CPU, memory, and disk storage. If the server runs out of resources, applications may become slow or stop working properly. Monitoring the host helps prevent performance problems and service interruptions.

Second, the `docker logs` command helps troubleshoot login problems by showing application messages, errors, and requests handled by a container. These logs can help identify possible causes, such as failed requests or application errors. By reviewing the logs, an engineer can investigate the problem instead of guessing what happened.

Third, monitoring logs and monitoring metrics have different purposes. Logs provide details about events, requests, and errors that happen inside an application. Metrics provide numerical information about performance, such as CPU usage, memory consumption, and network activity. Both are important because logs help explain what happened, while metrics show how the container is performing.

Fourth, large enterprise companies can monitor thousands of containers using centralized monitoring tools such as Prometheus and Grafana. Prometheus can collect and store metrics from different systems, while Grafana can display the information through dashboards and visualizations. These tools help engineers observe performance, identify unusual behavior, and respond to problems more efficiently.

Finally, my ability to troubleshoot Linux environments has improved through this laboratory. I learned how to check memory and disk usage, view running processes, deploy an Nginx container, test HTTP requests, read application logs, and monitor container resources using Docker commands. This activity helped me become more confident in using the terminal and understand the responsibilities of a Cloud Operations Engineer.
