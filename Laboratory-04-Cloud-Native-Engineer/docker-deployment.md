# Docker Environment

The Docker environment was accessed through the KillerCoda Playground. Before deploying the Nginx web server, I checked if Docker was installed and running.

## 1. Check Docker Version

* docker --version

This command displays the installed Docker version.

## 2. Check Docker Environment

* docker info

This command displays detailed information about the Docker environment and helps confirm that the Docker service is running.

## 3. Pull the Nginx Image

* docker pull nginx

This command downloads the official Nginx image from Docker Hub so it can be used to create a container.

## 4. Run the Nginx Container

* docker run -d -p 8080:80 --name nginx-server nginx

This command creates and runs an Nginx container in detached mode. The `-p 8080:80` option maps port 8080 on the host machine to port 80 inside the Nginx container.

## 5. Test the Web Server

* curl http://localhost:8080

This command sends an HTTP request to the Nginx server through port 8080. A successful deployment should display the HTML code of the Nginx welcome page.

## 6. List Running Containers

* docker ps

This command displays the currently running Docker containers.

## 7. Stop the Container

* docker stop nginx-server

This command stops the running Nginx container.

## 8. Verify the Container Is Stopped

* docker ps -a

This command displays all containers, including stopped containers, allowing me to verify that the Nginx container is no longer running.

## 9. Remove the Container

* docker rm nginx-server

This command completely removes the stopped Nginx container.

