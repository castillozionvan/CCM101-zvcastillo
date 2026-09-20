# Laboratory Activity 5: The Cloud Data Engineer

## Mission Overview
In this laboratory activity, I stepped into the role of a Cloud Data Engineer at CloudNova Technologies. The goal was to deploy a local, high-performance, S3-compatible Object Storage server using MinIO inside a Docker container on the KillerCoda environment. This activity highlights why object storage is essential for modern cloud-native applications dealing with massive volumes of unstructured data like images and media backups.

## Objectives
- Differentiate between Block, File, and Object Storage mechanisms.
- Deploy an S3-compatible MinIO Object Storage server using Docker containerization.
- Access containerized web services via port forwarding (Port `9001`).
- Configure cloud storage buckets and upload object data via a web management console.
- Document technical configurations and operations cleanly using Markdown.

## Tools Used
- **Docker**: Containerization engine used to pull and run the MinIO server image.
- **MinIO**: High-performance, S3-compatible object storage software.
- **KillerCoda Playground**: Cloud-based Linux/Ubuntu environment.
- **GitHub**: Version control system hosting this cloud portfolio.
- **Markdown**: Document formatting standard for technical reports.

## Skills Learned
- Configuring environment variables (`-e`) in Docker runtime parameters.
- Exposing and mapping multiple container ports (`9000` for API, `9001` for Console).
- Object Storage management: Bucket creation, access management, and object uploads.
- Evaluating cloud storage architectures (Block vs. File vs. Object) for real-world application demands.

---

## Deliverables & Evidence

### Storage Architecture Research
Detailed theoretical analysis is located in [`storage-types-research.md`](./storage-types-research.md).

### Technical Deployment Details
Detailed technical logs and command breakdowns are located in [`minio-deployment.md`](./minio-deployment.md).

### Reflection
Personal analysis and answers to mission reflection questions are located in [`reflection.md`](./reflection.md).

### Screenshots
| Verification Task | Screenshot Evidence |
| :--- | :--- |
| **MinIO Container Running** | `![MinIO Deployed](./screenshots/minio-deployed.png)` |
| **Bucket Creation & File Upload** | `![MinIO Bucket & Upload](./screenshots/minio-bucket-upload.png)` |
