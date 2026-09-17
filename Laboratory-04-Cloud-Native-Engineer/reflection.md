# Mission Reflection

This laboratory activity helped me understand how containerization makes application deployment faster and easier compared to using traditional Virtual Machines. A Docker container can start in seconds because it does not need to install and boot a complete operating system. In contrast, setting up a Virtual Machine usually requires installing an operating system and allocating more resources before the application can be used. This made me realize why containers are useful for applications that need quick deployment.

The port mapping `-p 8080:80` is necessary because the Nginx web server is running inside the container on port 80. Port mapping connects port 8080 on the host machine to port 80 inside the container. Because of this mapping, I was able to access the Nginx web server using `http://localhost:8080`. Without port mapping, the web server inside the container would not be directly accessible through the host port used in the activity.

When the `docker rm` command is used, the container itself is removed. Any data stored inside the container that is not saved outside the container can be lost. This showed me that containers are meant to be temporary and that important data should be stored separately when it needs to be preserved.

Containerization can also improve collaboration between software developers and IT operations teams. Developers can package an application and its required environment into a container, while operations teams can deploy and manage the same containerized application. This can make the development and deployment process more consistent and support the DevOps approach.

My GitHub portfolio is also evolving as I continue adding laboratory activities and documenting what I have learned. Instead of only storing files, it is becoming a record of my practical cloud computing skills. Each laboratory adds new commands, concepts, screenshots, and documentation that show my progress as an Information Technology student.
