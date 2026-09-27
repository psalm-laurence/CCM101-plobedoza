# Reflection

This activity helped me understand how useful Docker Compose is when working with multiple containers. Instead of running many commands to create and configure each container separately, I can put the settings in a `docker-compose.yml` file and use one command to start the whole application. This makes the process easier and faster, especially when I need to set up the same application again.

I also learned that YAML is very sensitive to indentation. Using the wrong spaces or a Tab can cause errors when Docker Compose reads the file. At first, I thought the formatting was simple, but I realized that even a small indentation mistake can stop the whole configuration from working.

I also learned how environment variables are used in the Compose file. Variables like `MYSQL_PASSWORD`, `MYSQL_DATABASE`, and `MYSQL_USER` provide the information that Nextcloud needs to connect to the MariaDB database. This makes the configuration easier to manage because the needed settings are already provided when the containers start.

It was also interesting to see a private cloud storage system like Nextcloud running after just a few setup steps. Before this activity, I thought setting up a cloud application would be much more complicated. Using Docker Compose showed me that having a proper configuration file can make the deployment process much simpler.

Since Mission 1, my understanding of Cloud Computing has improved. I started by learning basic Linux commands and cloud infrastructure, and now I have experience with Docker, containers, object storage, and multi-container applications. I also have a better idea of how these technologies work together. These activities also helped me become more comfortable with the Linux terminal and documenting my work using GitHub.

