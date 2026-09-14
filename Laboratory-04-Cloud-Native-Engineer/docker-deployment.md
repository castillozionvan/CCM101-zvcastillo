# Docker Container Lifecycle Documentation

## Overview
This document logs the step-by-step Docker CLI commands executed during Laboratory 04 to pull, run, verify, manage, and remove an Nginx containerized web server inside the KillerCoda environment.

## Lifecycle Commands & Descriptions

1. `docker --version`
   - **Explanation:** Verified that the Docker engine client and server components are installed and displayed their operational version details.

2. `docker info`
   - **Explanation:** Displayed system-wide information regarding the Docker installation, including running containers, active images, storage drivers, and system resources.

3. `docker pull nginx`
   - **Explanation:** Downloaded the latest official Nginx image from Docker Hub to the local host storage.

4. `docker run -d -p 8080:80 --name my-nginx nginx`
   - **Explanation:** Started a new container named `my-nginx` in detached mode (`-d`) in the background, mapping host port 8080 to container port 80 (`-p 8080:80`).

5. `curl http://localhost:8080`
   - **Explanation:** Sent an HTTP GET request to local port 8080 to verify that the Nginx web server inside the container was running and serving web traffic properly.

6. `docker ps`
   - **Explanation:** Listed all currently running containers on the host machine to verify container status, health, uptime, and mapped ports.

7. `docker stop my-nginx`
   - **Explanation:** Gracefully stopped the running `my-nginx` container by sending a SIGTERM signal to its main process.

8. `docker ps -a`
   - **Explanation:** Listed all containers on the host system (including stopped ones), confirming that `my-nginx` had entered an `Exited` state.

9. `docker rm my-nginx`
   - **Explanation:** Permanently removed the stopped `my-nginx` container and its top writable layer from host storage.
