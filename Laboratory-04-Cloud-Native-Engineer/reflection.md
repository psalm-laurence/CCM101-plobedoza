# Reflection

This activity helped me understand the difference between using a virtual machine and using a Docker container. When using a VM, setting up the operating system can take a lot of time and resources because the VM needs its own operating system. In Docker, a container can start in just a few seconds because it is much more lightweight. This made me realize why containers are commonly used when applications need to be deployed quickly.

I also learned why port mapping is important when running a web server. The -p 8080:80 command connects port 8080 of the host machine to port 80 inside the container. Without this mapping, I would not be able to access the Nginx web server through localhost:8080. Using the curl command allowed me to check if Nginx was running successfully.

Another thing I learned was what happens when a container is removed using docker rm. The container and its data inside its writable layer are removed. This means important data should not simply be stored inside the container if it needs to be kept. Docker volumes can be used when data needs to remain even after the container is deleted.

Containerization can also help developers and IT operations teams work better together. Developers can package an application with its required files and dependencies, while IT teams can run the same container in different environments. This makes deployment easier and helps avoid problems caused by different system setups.

Finally, this activity helped improve my GitHub portfolio. I was able to add my Docker commands, screenshots, comparison of VMs and containers, and my reflection. It shows my progress in learning cloud computing and basic container management. Overall, this activity gave me a better understanding of why Docker is useful in modern cloud environments.

