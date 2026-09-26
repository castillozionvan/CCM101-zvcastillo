# Laboratory 06: Cloud Deployment Engineer

## Mission Overview
In this laboratory activity, I transitioned from imperative manual container commands to declarative **Infrastructure as Code (IaC)** using Docker Compose. Using a YAML configuration file, I defined and deployed a two-tier enterprise cloud storage application consisting of a **Nextcloud** web container and a **MariaDB** backend database, orchestrating the entire stack simultaneously with a single command.

---

## Objectives
* Explain the concepts and benefits of a multi-tier application architecture.
* Understand the purpose, syntax, and structure of a `docker-compose.yml` file.
* Utilize command-line text editors (`nano`) to construct valid Infrastructure as Code blueprints.
* Deploy and tear down multi-container stacks in detached mode (`docker-compose up -d` and `docker-compose down`).
* Document deployment procedures, service discovery mechanisms, and IaC principles using Markdown.
* Expand the professional GitHub Cloud Computing Portfolio.

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
