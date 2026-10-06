# Laboratory Activity 5: The Cloud Data Engineer

## Mission Overview
Congratulations! Your seamless deployment of containerized web servers has caught the attention of
the senior architects. You have now been temporarily reassigned to the Cloud Data Engineering Team at
CloudNova Technologies.
In the cloud, data is everything. However, not all data is stored the same way. While traditional
computers use hard drives (Block Storage) and shared network drives (File Storage), modern cloud applications
rely heavily on Object Storage to store massive amounts of unstructured data like images, videos, and backups.
The industry standard for this is Amazon S3, but today, you will deploy your very own S3-compatible cloud
storage server using an open-source tool called MinIO.
Using your KillerCoda Playground, you will combine your new Docker skills with your cloud storage knowledge to
deploy a live object storage server, create a storage "bucket," and upload data over the web.
Remember: A cloud engineer doesn't just store data; they ensure it is scalable, accessible, and secure.


## Objectives
At the end of this laboratory activity, you should be able to:
- Differentiate between Block, File, and Object Storage.
- Deploy an S3-compatible Object Storage server (MinIO) using Docker.
- Access a cloud service via a web interface using port forwarding.
- Create a storage bucket and upload objects (files) to the cloud.
- Document cloud storage operations using Markdown.
- Continue expanding a professional GitHub Cloud Computing Portfolio. 

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


