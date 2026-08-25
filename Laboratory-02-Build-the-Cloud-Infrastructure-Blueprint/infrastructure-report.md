# Cloud Server Infrastructure Investigation Report

## System Specifications

| Parameter | Value / Finding |
| :--- | :--- |
| **Operating System** | Ubuntu 24.04.4 LTS |
| **Kernel Version** | 6.8.0-138-generic |
| **CPU Model** | Intel Xeon E312xx (Sandy Bridge, IBRS update) RHEL-9.6.0 PC (Q35 + ICH9, 2009) CPU @ 2.0GHz |
| **Number of CPU Cores** | 1 |
| **Total RAM** | 1.9 GB |
| **Disk Capacity** | 19 GB |
| **Mounted File Systems** | **Filesystem** &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Type** &nbsp;&nbsp;&nbsp;&nbsp; **Size** &nbsp;&nbsp; **Used** &nbsp; **Avail** &nbsp; **Use%** &nbsp; **Mounted on**<br>tmpfs &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; tmpfs &nbsp;&nbsp; 191M &nbsp;&nbsp; 996K &nbsp;&nbsp; 190M &nbsp;&nbsp;&nbsp; 1% &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; /run<br>/dev/vda1 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ext4 &nbsp;&nbsp;&nbsp;&nbsp; 19G &nbsp;&nbsp;&nbsp;&nbsp; 5.4G &nbsp;&nbsp;&nbsp; 13G &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 30% &nbsp;&nbsp;&nbsp; /<br>tmpfs &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; tmpfs &nbsp;&nbsp; 952M &nbsp;&nbsp; 84K &nbsp;&nbsp;&nbsp;&nbsp; 952M &nbsp;&nbsp;&nbsp; 1% &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; /dev/shm<br>tmpfs &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; tmpfs &nbsp;&nbsp; 5.0M &nbsp;&nbsp; 0 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 5.0M &nbsp;&nbsp;&nbsp; 0% &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; /run/lock<br>/dev/vda16 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ext4 &nbsp;&nbsp;&nbsp;&nbsp; 881M &nbsp;&nbsp; 117M &nbsp;&nbsp; 703M &nbsp;&nbsp;&nbsp; 15% &nbsp;&nbsp;&nbsp; /boot<br>/dev/vda15 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; vfat &nbsp;&nbsp;&nbsp;&nbsp; 105M &nbsp;&nbsp; 6.2M &nbsp;&nbsp;&nbsp; 99M &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 6% &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; /boot/efi |
| **Hostname** | ubuntu |
| **IP Address** | 172.30.1.2, 172.17.0.1 |
