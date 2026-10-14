# Security Audit Report: Core Principles & Threat Modeling

## 1. The Principle of Least Privilege (PoLP)
The Principle of Least Privilege dictates that a user, program, or process should only have the bare minimum permissions necessary to perform its intended function and nothing more. In cloud user accounts, this is crucial because if an attacker compromises a specific service account or IAM user credential, the scope of the breach is strictly contained rather than granting full administrative control over the entire cloud infrastructure.

## 2. Attack Surface
An attack surface refers to the sum total of all vulnerable entry points—such as open network ports, exposed APIs, misconfigured storage buckets, and running services—where an unauthorized user can try to enter or extract data from a virtual machine. When applied to a cloud server, every unnecessary service running or port left open directly expands this surface, increasing the probability of a successful exploit.

## 3. Default Deny Policy
A Default Deny policy is a security posture where all inbound and outbound traffic is blocked by default, and only explicitly approved exceptions are allowed to pass through. It is significantly safer than trying to block specific malicious actors individually because attackers constantly change IP addresses and exploit new vectors; a default deny ensures that unknown or unauthorized traffic is dropped automatically.
