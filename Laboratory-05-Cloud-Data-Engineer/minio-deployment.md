# MinIO Deployment

## 1. Deploy MinIO Using Docker

I used Docker to download and run the MinIO object storage server.

` docker run -d -p 9000:9000 -p 9001:9001 --name minio-server -e "MINIO_ROOT_USER=cloudadmin" -e "MINIO_ROOT_PASSWORD=CloudNova2026!" minio/minio server /data --console-address ":9001" `


The command creates a MinIO container and runs it in detached mode.

## 2. Verify the Container

I used the following command to check if the MinIO container was running:

` docker ps `


This command displays the currently running Docker containers. The MinIO container should have a status showing that it is running.

## 3. Access the MinIO Web Console

The MinIO Web Console was accessed using:

` Port: 9001 `
 

Port 9001 was mapped from the host to the MinIO Web Console port.

## 4. MinIO Login Credentials

The credentials were defined using environment variables in the Docker command.


` Username: cloudadmin
Password: CloudNova2026! `


## 5. Environment Variables

The `-e` flags are used to set environment variables inside the Docker container.

` -e "MINIO_ROOT_USER=cloudadmin" `

This sets the MinIO administrator username.

` -e "MINIO_ROOT_PASSWORD=CloudNova2026!" `

This sets the MinIO administrator password.

Using environment variables allows the MinIO container to receive its configuration when it starts.

## 6. Bucket Created

The storage bucket created for the client was:

` client-photos `

The bucket was created through the MinIO Web Console and a sample file was uploaded successfully.

## 7. Ports Used

| Port | Purpose           |
| ---- | ----------------- |
| 9000 | MinIO API         |
| 9001 | MinIO Web Console |

## 8. Result

The MinIO server was successfully deployed using Docker. I was able to access the Web Console, create the `client-photos` bucket, and upload a sample file.
