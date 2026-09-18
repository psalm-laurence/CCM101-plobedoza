# Reflection

This activity helped me understand why object storage is useful for applications that need to handle a large amount of data. For a photo-sharing application, storing millions of images on traditional block storage can become difficult to manage as the data continues to grow. Object storage is designed for large amounts of unstructured data such as photos, videos, and backups. It also makes it easier to access and organize these files.

Using Docker made the deployment of MinIO much easier. Instead of manually installing and configuring a storage server, I only needed to run a Docker command with the required settings. The container started quickly, and I was able to access the MinIO Web Console using the assigned port. This was similar to my previous Docker activity and helped me become more comfortable with using Docker commands.

I also learned that a bucket is a container used to organize and store objects in object storage. In this activity, I created a bucket named `client-photos` and uploaded a sample file into it. This gave me a better idea of how cloud storage can be used by applications to store user files.

For large companies, I think protecting object storage data involves using backups, replication, and multiple storage servers or locations. This helps prevent data loss if a physical server fails. Cloud providers can also use redundancy so that data remains available even when some hardware has problems.

My confidence in using the Linux command line is also improving. At first, Docker commands were unfamiliar to me, but after using commands like `docker run` and `docker ps`, I am becoming more comfortable working in the terminal. This activity also helped me connect Linux, Docker, cloud storage, and GitHub documentation together.

