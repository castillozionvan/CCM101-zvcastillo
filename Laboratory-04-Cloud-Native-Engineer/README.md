# Laboratory 04: Cloud-Native Engineer

## Mission Overview
Congratulations! After successfully guiding our clients through multi-cloud evaluations, you have been promoted to the Cloud-Native Engineering Team at CloudNova Technologies.

Modern cloud computing is no longer just about renting Virtual Machines (VMs) from AWS or Azure. Today's enterprise applications are built using lightweight, portable, and lightning-fast technologies called Containers.

Your new mission is to understand the shift from traditional virtualization to containerization. Using the KillerCoda Playground, you will step into the shoes of a Cloud-Native Engineer. You will research the differences between VMs and containers, execute your very first Docker commands, and deploy a live, containerized web server in seconds.

Remember: A traditional system administrator manages servers, but a cloud-native engineer manages the services running on them.

## Mission Objectives
At the end of this laboratory activity, you should be able to:
- Differentiate between traditional Virtual Machines (VMs) and Containers.
- Access a Docker-enabled cloud environment using KillerCoda.
- Execute fundamental Docker CLI (Command Line Interface) commands.
- Pull, run, manage, and terminate a containerized application (Nginx).
- Create professional technical documentation of container operations using Markdown.
- Continue developing a well-organized GitHub Cloud Computing Portfolio.

## Docker Commands Executed
```bash
docker --version
docker info
docker pull nginx
docker run -d -p 8080:80 --name my-nginx nginx
curl http://localhost:8080
docker ps
docker stop my-nginx
docker ps -a
docker rm my-nginx


Skills Learned
Linux container management using Docker CLI.

Host-to-container port mapping (-p 8080:80).

Local API and endpoint verification with curl.

Writing structured technical documentation in Markdown.

Challenges Encountered
Understanding Port Mapping: Learning how host ports route traffic into isolated container namespaces.

Detached vs. Interactive Mode: Differentiating between background execution (-d) and interactive terminal access (-it).
