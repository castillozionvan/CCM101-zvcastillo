# Laboratory 04: Cloud-Native Engineer

## Mission Overview
This laboratory activity introduces core containerization concepts using Docker. It covers the architectural differences between virtual machines and containers, practical deployment of microservices, networking port exposure, container lifecycle management, and clear technical documentation.

## Objectives
- Compare the architectural advantages of containers over traditional VMs.
- Verify Docker installation and daemon status in a Linux environment.
- Deploy, map ports, and test an Nginx web server using Docker CLI.
- Manage container lifecycles (pulling, running, stopping, and removing).
- Structure and document technical cloud workflows on GitHub.

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
