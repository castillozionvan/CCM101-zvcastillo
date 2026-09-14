# Mission Reflection

The boot time and setup process of a Docker container are vastly superior to setting up a traditional Virtual Machine. Installing an operating system on a VM requires allocating virtual hardware, loading an ISO file, and completing a full OS setup, which can take anywhere from 10 to 15 minutes. In contrast, Docker containers leverage the host system's shared OS kernel and run as isolated processes. This allows a container like Nginx to spin up and become fully operational in just a few seconds.

Port mapping using the `-p 8080:80` flag is essential because Docker containers run inside isolated network namespaces by default. Without port mapping, incoming traffic from the host machine cannot reach the web server listening inside the container. Using `-p 8080:80` explicitly bridges host port 8080 to container port 80, allowing us to access the Nginx web server locally via `http://localhost:8080`.

When you execute the `docker rm` command, the stopped container and its top writable layer are permanently deleted from host storage. Any temporary data written to the container's file system during its execution is completely destroyed unless persisted using an external Docker volume or bind mount.

Containerization transforms the relationship between software developers and IT operations teams within a DevOps culture. By packaging application code alongside its specific dependencies and runtime configs into a single immutable container image, developers eliminate the classic "it works on my machine" problem. Operations teams can reliably deploy the exact same container artifact to staging or production without encountering environment inconsistencies.

Through this activity, my GitHub portfolio is evolving from static cloud design architecture to active, hands-on cloud-native engineering. Successfully managing container lifecycles and exposing network ports demonstrates my growing technical capability in modern DevOps practices.
