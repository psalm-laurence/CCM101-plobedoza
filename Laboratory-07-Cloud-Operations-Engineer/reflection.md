# Reflection

This activity helped me understand why checking the host server is important even when the containers themselves are running normally. A container can be working properly, but the host server could still have high CPU usage, low memory, or limited disk space. Checking these resources gives the Cloud Operations Engineer an idea of whether the server can handle more workload and helps prevent possible problems.

I also learned how useful the `docker logs` command can be when troubleshooting an application. If a user cannot log into a web application, I can check the container logs to see if there are errors or failed requests. The logs can give information about what happened and can help narrow down the possible cause of the problem instead of just guessing.

Logs and metrics are also different types of monitoring information. Logs show specific events that happened in the application, such as HTTP requests and errors. Metrics provide numerical information about the system, such as CPU usage, memory usage, and network activity. Using both is useful because they give different views of the application's health.

For large companies with thousands of containers, manually checking every container would not be practical. They can use monitoring and observability tools such as Prometheus and Grafana to collect, organize, and display metrics from many systems in one place. These tools can help engineers notice problems more quickly and monitor large cloud environments.

My troubleshooting skills in Linux have also improved compared to when I started the first mission. I am now more comfortable using commands to check system resources, run Docker containers, generate requests, and inspect logs. I have learned that troubleshooting is not just about finding an error but also collecting information and using that information to understand what is happening. This activity made me more confident working with Linux and Docker.
