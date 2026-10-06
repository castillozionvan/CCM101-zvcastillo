# Laboratory 07: The Cloud Operations Engineer

## Mission Overview
Congratulations! Your ability to deploy multi-tier architectures has proven your technical capabilities.
You have now been promoted to the Cloud Operations Team (often referred to in the industry as Site Reliability
Engineering, or SRE) at CloudNova Technologies.
Deploying a cloud application is only the first step; keeping it running smoothly is the real challenge.
When a server crashes or a web page takes ten seconds to load, you cannot simply guess what is wrong. You
must rely on Observability and Monitoring to see inside your infrastructure.
Using the KillerCoda Playground, you will step into the role of a Cloud Operations Engineer. You will
establish a performance baseline for your Linux server, deploy a containerized application, generate artificial web
traffic, and hunt down performance metrics and system logs to prove the application is healthy.
Remember: A developer hopes the application works; a Site Reliability Engineer uses metrics and logs to
prove it.


## Objectives
At the end of this laboratory activity, you should be able to:
 Utilize native Linux command-line tools to monitor host CPU, Memory, and Disk capacity.
 Deploy a web container and track its real-time performance using Docker metrics.
 Generate web traffic and extract application access logs for analysis.
 Translate raw performance data into a readable technical report using Markdown.
 Continue expanding a professional GitHub Cloud Computing Portfolio. 

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
