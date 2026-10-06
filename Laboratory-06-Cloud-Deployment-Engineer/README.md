# Laboratory 06: Cloud Deployment Engineer

## Mission Overview
Congratulations! Your flawless work in deploying data storage solutions has earned you a spot on the
Cloud Deployment Team at CloudNova Technologies.
Up until now, you have been deploying single containers (like a standalone web server or a storage
bucket). However, real-world enterprise applications are rarely just one container. They are "multi-tier" systems
that require a frontend web application communicating seamlessly with a backend database. Deploying these
one by one manually is prone to error.
Enter Docker Compose. In this mission, you will transition from manual commands to Infrastructure
as Code (IaC). Using a YAML configuration file, you will define a multi-container private cloud storage application
(Nextcloud and MariaDB) and deploy the entire stack simultaneously with a single command!
Remember: A junior engineer deploys servers by typing commands; a senior engineer deploys
infrastructure by writing code.

---

## Objectives
At the end of this laboratory activity, you should be able to:
- Explain the concept of a multi-tier application architecture.
- Understand the purpose and structure of a docker-compose.yml file.
- Use a Linux command-line text editor (nano) to create configuration files.
- Deploy a multi-container application (Nextcloud + Database) using Docker Compose.
- Document deployment procedures and Infrastructure as Code (IaC) principles using Markdown.
- Continue expanding your professional GitHub Cloud Computing Portfolio. 
---

## Skills Learned 

1. Infrastructure as Code (IaC):
   - Translating multi-container architecture requirements into declarative YAML blueprints.
   - Managing application infrastructure programmatically rather than manually executing commands.

2. Service Discovery & Networking:
   - Establishing seamless inter-container communication across virtual bridge networks.
   - Using Docker internal DNS resolution to connect services via service names (e.g., MYSQL_HOST=database).

3. Container Lifecycle & Orchestration:
   - Executing multi-container deployment, monitoring, and teardown using Docker Compose CLI commands (docker-compose up -d, ps, down).
   - Port forwarding containerized application ports to host interfaces for browser access.

## Commands Executed

```bash
# 1. Create project working directory
mkdir nextcloud-deployment
cd nextcloud-deployment

# 2. Construct Infrastructure as Code file
nano docker-compose.yml

# 3. Deploy multi-container application stack in detached mode
docker-compose up -d

# 4. Verify running services and status
docker-compose ps

# 5. Terminate and gracefully remove container stack
docker-compose down
