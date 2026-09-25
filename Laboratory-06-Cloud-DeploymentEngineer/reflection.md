# Mission Reflection

Writing a `docker-compose.yml` file makes a cloud engineer's job easier because it allows the configuration of multiple containers to be written in one file. Instead of manually typing many Docker commands, Docker Compose can create and manage the application stack using the instructions in the YAML file. This makes the deployment more organized, repeatable, and easier to manage.

I also learned that YAML is very sensitive to indentation. When I first created my Compose file, I encountered an error because the indentation was incorrect. The `docker-compose config` command showed a YAML scanner error, which helped me understand that spaces are important in YAML. Using a Tab instead of the correct spaces or placing a line at the wrong level can prevent Docker Compose from reading the configuration.

Environment variables such as `MYSQL_PASSWORD` are used to provide configuration values to the containers. In this activity, they allowed the Nextcloud application and MariaDB database to use the required database credentials and settings without placing those values directly into the application commands.

Deploying Nextcloud in only a few minutes was a good experience because I was able to see how several components can work together as one cloud application. Seeing the Nextcloud setup page in the browser also showed me that the containers were communicating successfully.

Since Mission 1, my understanding of Cloud Computing has developed from learning basic cloud concepts to actually deploying and managing infrastructure. I now have a better understanding of containers, multi-tier architecture, Docker Compose, Infrastructure as Code, and the importance of documenting deployment procedures.