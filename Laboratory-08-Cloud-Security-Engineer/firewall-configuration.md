# UFW Firewall Configuration & Execution Log

## Step-by-Step Commands Executed

### 1. Allow Secure Shell (SSH) Access
To prevent getting locked out of the remote server once the firewall is enabled, SSH traffic on port 22 must be allowed first:

sudo ufw allow ssh

---

### 2. Configure Default Policies
Enforce a baseline security posture by denying all incoming connections by default while allowing outbound traffic for system updates and package fetching:

sudo ufw default deny incoming
sudo ufw default allow outgoing

---

### 3. Enable the Firewall
Activate the Uncomplicated Firewall (UFW) service:

sudo ufw enable

(Note: Press 'y' when prompted to proceed with enabling the firewall active on system startup).

---

### 4. Verify Firewall Status
Check the verbose status to confirm rules and default policies:

sudo ufw status verbose

---

### 5. Granular Port Management (Web Application)
Allow targeted TCP traffic on port 8080 for the Nginx containerized web service:

sudo ufw allow 8080/tcp
sudo ufw status numbered

---

## Critical Safety Note

What would happen if you ran "sudo ufw enable" before running "sudo ufw allow ssh"?
Running "sudo ufw enable" before permitting SSH would instantly drop all active inbound connections on port 22, permanently locking you out of the remote server session and requiring physical or hypervisor-level console intervention to regain access.
