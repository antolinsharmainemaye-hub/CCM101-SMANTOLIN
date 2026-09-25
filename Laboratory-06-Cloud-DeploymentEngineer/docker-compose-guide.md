# Docker Compose Guide

## What does the `services:` block do?

The `services:` block defines the containers that make up the application. In our Docker Compose file, there are two services: `database` and `app`. The `database` service uses the MariaDB image, while the `app` service uses the Nextcloud image. Docker Compose uses these definitions to create and manage the containers as one application stack.

## How does the Nextcloud app container find the database container?

The Nextcloud app container finds the database through the `MYSQL_HOST` environment variable. In our Compose file, we set:

`MYSQL_HOST=database`

The value `database` refers to the name of the database service in the `services:` block. This allows the Nextcloud container to communicate with the MariaDB database container using its service name.

## Difference Between `docker run` and `docker-compose up -d`

The `docker run` command is used to create and run an individual Docker container. It is useful when deploying a single container manually.

In contrast, `docker-compose up -d` uses the configuration in the `docker-compose.yml` file to create and start multiple related containers as one application stack. The `-d` option runs the containers in detached mode, allowing them to continue running in the background while the terminal is available for other commands.