# Docker Compose Guide

## Docker Compose File

The `docker-compose.yml` file is used as a blueprint for deploying the Nextcloud application and MariaDB database together.

```yaml
version: '3'

services:
  database:
    image: mariadb:10.6
    environment:
      - MYSQL_ROOT_PASSWORD=cloudnova_root
      - MYSQL_PASSWORD=cloudnova_pass
      - MYSQL_DATABASE=nextcloud_db
      - MYSQL_USER=nextcloud_user

  app:
    image: nextcloud
    ports:
      - 8080:80
    environment:
      - MYSQL_PASSWORD=cloudnova_pass
      - MYSQL_DATABASE=nextcloud_db
      - MYSQL_USER=nextcloud_user
      - MYSQL_HOST=database
```

## The `services:` Block

The `services:` block defines the containers that make up the application. In this project, there are two services: `database` for MariaDB and `app` for Nextcloud.

The database service provides the database, while the app service provides the Nextcloud web application.

## How Nextcloud Finds the Database

The Nextcloud container uses the following environment variable:

```yaml
- MYSQL_HOST=database
```

The value `database` matches the name of the MariaDB service in the Compose file. Docker Compose creates a network for the services, allowing the Nextcloud container to communicate with the database using the service name.

## Difference between `docker run` and `docker-compose up -d`

The `docker run` command is normally used to create and start one Docker container at a time. I used this approach in previous activities when deploying containers such as Nginx and MinIO.

The `docker-compose up -d` command can deploy multiple related containers based on a Compose YAML file. Instead of entering many commands manually, the configuration is written once in the file and Docker Compose uses it to create and start the complete application stack.

