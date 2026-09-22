# MinIO Deployment - Technical Documentation

## Docker Command Used

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \
-e "MINIO_ROOT_USER=cloudadmin" \
-e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
minio/minio server /data --console-address ":9001"
This command deployed the MinIO object storage server using Docker and exposed the API and Web Console ports.

Web Console Port

The MinIO Web Console was accessed using:

9001

Port 9001 allows access to the MinIO management interface through a web browser.

Bucket Created

The storage bucket created during the activity was:

client-photos

This bucket was used to store the sample file uploaded during the activity.

Environment Variables

The -e flags are used to set environment variables inside the Docker container. In this deployment, MINIO_ROOT_USER set the administrator username to cloudadmin, while MINIO_ROOT_PASSWORD set the administrator password used to log in to the MinIO Web Console.