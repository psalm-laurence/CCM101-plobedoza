# Container Observability

## Application Logs

I retrieved the Nginx container logs using:

``docker logs client-website``

The logs showed the HTTP requests sent to the Nginx web server, including successful requests and the request that resulted in a 404 error.

### 404 Error Log

The following line shows the 404 request:

``172.17.0.1 - - [05/Oct/2026:10:16:48 +0000] "GET /hidden-admin-page HTTP/1.1" 404 153 "-" "curl/8.5.0" "-"``

Application logs are important because they show what happened when users interacted with an application. They can help engineers identify errors and understand what happened before a problem occurred.

## Real-Time Container Metrics

I used the following command to monitor the container:

``docker stats``

The `docker stats` command displays real-time resource usage for running containers.

At the time of my observation, the `client-website` container was using:

- **CPU:** 0.00%
- **Memory Usage:** 2.73MiB / 1.895GiB

The CPU and memory values provide information about how much of the host's resources the container is consuming.

## Observability Summary

Logs and metrics provide different types of information. Logs show specific events and requests that happened inside the application, while metrics provide numerical information about resource usage and performance. Using both allows a Cloud Operations Engineer to better understand the health of a containerized application.
