# Laboratory 07: The Cloud Operations Engineer

## Mission Overview
This laboratory activity focuses on system observability, monitoring, and health verification for containerized cloud applications. As part of the Site Reliability Engineering (SRE) team at CloudNova Technologies, this mission establishes a host hardware performance baseline, deploys an Nginx web application, generates synthetic traffic, and analyzes application logs alongside real-time metrics.

## Objectives
* Establish host hardware baselines (CPU, Memory, Disk) using native Linux commands.
* Deploy a containerized web server and track real-time resource utilization via Docker metrics.
* Simulate normal and error-inducing HTTP web traffic using `curl`.
* Extract and evaluate application access logs to detect error status codes.
* Document system metrics and technical observations in structured Markdown reports.

## Monitoring Commands Executed
| Command | Purpose |
| :--- | :--- |
| `free -h` | Displays total, used, and available system memory (RAM). |
| `df -h /` | Inspects disk space usage and available capacity on the root filesystem. |
| `top` | Opens a real-time process manager displaying CPU usage and system load. |
| `docker run -d --name client-website -p 8080:80 nginx` | Runs Nginx container detached on port 8080. |
| `curl http://localhost:8080/<path>` | Sends synthetic HTTP GET requests to generate log entries. |
| `docker logs client-website` | Fetches container access and error stdout/stderr streams. |
| `docker stats` | Streams live container resource consumption (CPU, Memory, Network I/O). |

## Skills Learned
* Host level health inspection using `free`, `df`, and `top`.
* Application lifecycle management and containerized deployment using Docker.
* HTTP log parsing and status code identification (`200 OK`, `404 Not Found`).
* SRE observability practices differentiating logs (events) from metrics (time-series performance).
