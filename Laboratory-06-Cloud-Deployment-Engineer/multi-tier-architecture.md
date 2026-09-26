# Multi-Tier Architecture: Nextcloud & MariaDB

## Definition of Two-Tier Architecture
A **Two-Tier Architecture** is a software design pattern where an enterprise application is divided into two separate functional layers: a presentation/application layer (web server) and a data storage layer (database). Each layer operates independently within its own container and communicates across a secure private container network.

---

## Tiers Breakdown

### 1. The Web/Application Tier
* **Role:** Serves as the primary user interface and application processing layer.
* **Function:** Handles incoming HTTP/HTTPS user requests, serves the Nextcloud web interface, processes PHP application logic, and communicates with the backend database tier to execute user requests.

### 2. The Database Tier
* **Role:** Provides persistent, relational data management and storage.
* **Function:** Stores critical application data, including user account credentials, system settings, access logs, directory indexes, and file metadata.

---

## Why Separate Them?

Separating the web application and database into two independent containers is superior to bundling them into a single container for three key reasons. First, it enables independent scaling, allowing engineers to scale out the web server tier to handle high web traffic without duplicating or locking the database. Second, it enhances security by isolating the database behind an internal network so that an exploit on the public-facing web tier does not directly compromise stored data. Finally, it improves maintainability, allowing developers to update, patch, or restart the web application without disrupting or corrupting the database service.
