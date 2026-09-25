# Two-Tier Architecture

A **Two-Tier Architecture** is a system architecture where the application is divided into two main tiers: the **Web/Application Tier** and the **Database Tier**. In this laboratory, the Nextcloud web application and MariaDB database are deployed as separate containers.

## The Web/Application Tier

The **Web/Application Tier** is responsible for serving the user interface and handling HTTP requests from users. In this laboratory, the **Nextcloud application container** serves as the Web/Application Tier.

## The Database Tier

The **Database Tier** is responsible for storing and managing persistent data. This includes **user accounts, credentials, and file metadata**. In this laboratory, the **MariaDB container** serves as the Database Tier.

## Why Separate Them?

Separating the web server and database into two containers makes the system easier to manage and maintain. Each container has a specific responsibility, and the database can operate separately from the web application. This also allows the two services to communicate through Docker Compose while keeping their roles separate.
