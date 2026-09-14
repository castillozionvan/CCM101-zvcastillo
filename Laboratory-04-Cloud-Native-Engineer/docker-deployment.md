# Docker Container Lifecycle Documentation

## Lifecycle Commands & Descriptions

1. `docker ps`
   - **Explanation:** Listed all currently running containers on the host machine along with their details such as Container ID, image name, created time, and active port mappings.

2. `docker stop my-nginx`
   - **Explanation:** Gracefully stopped the running `my-nginx` container by sending a SIGTERM signal to its main process.

3. `docker ps -a`
   - **Explanation:** Listed all containers on the host system including stopped ones, verifying that the `my-nginx` container was successfully stopped.

4. `docker rm my-nginx`
   - **Explanation:** Permanently removed the stopped `my-nginx` container from the local storage.
