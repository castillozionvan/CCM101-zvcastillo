# Laboratory 01: Welcome to the Cloud

## Mission Overview
Congratulations! 
You have been accepted as a Junior Cloud Infrastructure Engineer Trainee at CloudNova Technologies, a 
company specializing in cloud infrastructure, virtualization, and enterprise cloud solutions. 
As part of your onboarding process, you must complete your first mission. Before deploying cloud services or 
managing enterprise infrastructures, every cloud engineer must first learn how to work inside a Linux 
environment, document their work professionally, and maintain a version-controlled portfolio using GitHub. 
Your task is to complete the onboarding mission using the KillerCoda Playground and create your personal 
Cloud Computing Portfolio on GitHub. This portfolio will serve as your professional workspace throughout the 
semester and will be updated after every laboratory activity. 
Complete each checkpoint carefully. Every completed task represents a real-world responsibility of a cloud 
engineer.

## Mission Objectives
Upon successful completion of this mission, you should be able to: 
* Access a cloud-based Linux environment using KillerCoda. 
 Explore and navigate the Linux operating system. 
 Gather basic system information. 
 Organize files and directories using Linux commands. 
 Create and maintain a professional GitHub repository. 
 Document technical work using Markdown. 
 Demonstrate proper documentation practices used by cloud professionals.

## Activities Performed
1. Launched an Ubuntu 24.04 playground on KillerCoda.
2. Created a new user account `zvcastillo` with standard Bash access and `sudo` rights.
3. Extracted CPU, memory, OS release, kernel, and disk space information.
4. Created a workspace directory tree consisting of `Documents`, `Notes`, `Screenshots`, and `Reports`.
5. Created `system-information.md` and `about-me.md` markdown files.
6. Initialized the `CCM101-zvcastillo` repository and committed laboratory deliverables.

## Linux Commands Used
* `sudo useradd -m -s /bin/bash zvcastillo` – Added user with home directory and Bash shell.
* `sudo passwd zvcastillo` – Set account password.
* `sudo usermod -aG sudo zvcastillo` – Added user to administrative group.
* `su - zvcastillo` – Switched account session.
* `cat /etc/os-release` & `uname -r` – Retrieved OS distribution and kernel details.
* `lscpu`, `free -h`, `df -h` – Displayed CPU, memory, and disk utilization.
* `mkdir -p Workspace/{Documents,Notes,Screenshots,Reports}` – Built directory structure.
* `cat << 'EOF' > file.md` – Generated markdown documentation directly via terminal.

## Skills Learned
* Basic Linux user and access management.
* Command-line system auditing and resource tracking.
* POSIX file system navigation and file creation.
* Git version control integration for cloud documentation.
