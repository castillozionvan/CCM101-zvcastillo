# MinIO Object Storage Deployment Documentation

## 1. Deployment Execution Command
The MinIO object storage server was containerized and executed in the KillerCoda environment using the following Docker command:

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \
-e "MINIO_ROOT_USER=cloudadmin" \
-e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
minio/minio server /data --console-address ":9001"
