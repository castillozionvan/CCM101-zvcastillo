# Technical Documentation: Docker Compose Guide

## Key YAML Concepts & Architecture Explanation

### 1. What the `services:` Block Does
The `services:` top-level element in a `docker-compose.yml` file acts as the primary container registry block. It defines all the individual containerized components that make up the multi-tier application stack—in our deployment, the `database` service (MariaDB) and the `app` service (Nextcloud). Docker Compose automatically spins up each service defined here as an isolated container on a shared default virtual bridge network.

### 2. Service Discovery and Container Communication (`MYSQL_HOST`)
The Nextcloud application container communicates seamlessly with the MariaDB database container using the environment variable:
`MYSQL_HOST=database`

Docker Compose establishes a private network for all services in the file and provides built-in DNS service discovery. Instead of requiring static IP addresses—which change every time a container restarts—Docker’s internal DNS automatically resolves the service name `database` directly to the IP address assigned to the MariaDB container.

---

## Technical Comparison: `docker run` vs. `docker-compose up -d`

| Feature | `docker run` | `docker-compose up -d` |
| :--- | :--- | :--- |
| **Approach** | Imperative (Manual step-by-step CLI execution) | Declarative (Infrastructure as Code - IaC) |
| **Container Scope** | Deploys only one container per command | Deploys multi-container stacks simultaneously |
| **Configuration** | Long, error-prone CLI arguments (`-d`, `-p`, `-e`) | Clean, version-controlled `docker-compose.yml` file |
| **Networking** | Requires manual creation of custom bridge networks | Automatically builds a shared network with DNS resolution |
| **Lifecycle Control** | Containers must be started/stopped individually | The entire infrastructure stack is managed via single commands (`up`/`down`) |
