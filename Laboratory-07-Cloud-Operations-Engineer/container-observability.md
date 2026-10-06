# Container Observability & Monitoring Report

## Application Error Log Analysis

### Application logs serve as an essential audit trail that captures exact user actions, HTTP status codes, and runtime errors occurring within a container. They enable Site Reliability Engineers to pinpoint failing endpoints and debug application failures without guessing.
**Extracted 404 Error Log:**

## Real-Time Resource Metrics

* **Memory Usage:** `2.746MiB / 1.859GiB`
* **CPU Percentage:** `0.00%`
  
```log
172.17.0.1 - - [06/Oct/2026:04:53:05 +0000] "GET /hidden-admin-page HTTP/1.1" 404 153 "-" "curl/8.5.0" "-"
