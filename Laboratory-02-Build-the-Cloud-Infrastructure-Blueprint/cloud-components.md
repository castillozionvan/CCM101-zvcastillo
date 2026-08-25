# Identification of Cloud Infrastructure Components

## 1. Compute Resources
* **Purpose:** Process instructions, run application logic, and execute virtualized workloads in real-time.
* **Importance in Cloud:** Serves as the core engine that drives application hosting, scalable microservices, and serverless compute functions.
* **KillerCoda Relation:** Represented by the virtualized vCPU allocation running the KillerCoda interactive Linux shell container.

## 2. Storage Resources
* **Purpose:** Persistently or ephemerally hold file systems, OS binaries, user data, and system logs.
* **Importance in Cloud:** Guarantees data durability, enables high-speed block storage access for databases, and provides scalable object storage for web assets.
* **KillerCoda Relation:** Represented by the root block storage partition (`/`) mounted on `ext4` or `overlayfs` providing disk space for the environment.

## 3. Networking Resources
* **Purpose:** Enable data transmission, remote connections, route management, and security boundaries across distributed nodes.
* **Importance in Cloud:** Connects isolated instances to internal service meshes, public internet gateways, and secure VPN channels.
* **KillerCoda Relation:** Represented by the virtual Ethernet interface (`eth0`) assigned a private IP address for routing inbound/outbound TCP/UDP traffic.

## 4. Operating System
* **Purpose:** Manage low-level system hardware, allocate system resources, manage security access, and provide execution runtimes for applications.
* **Importance in Cloud:** Acts as the foundation layer for virtual machines and container host nodes, providing stability and security isolation.
* **KillerCoda Relation:** The Ubuntu Linux kernel and distribution underlying the interactive web shell environment.
