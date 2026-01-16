## Operating System Security Fundamentals (Linux & Windows)
Internship Task 2

## Overview
This document demonstrates operating system security fundamentals using Kali Linux. The objective of this task is to understand user privileges, file permissions, running services, firewall configuration, and operating system hardening in order to reduce the overall system attack surface.

The task focuses on practical, command-based implementation of OS security concepts.

---

## Objectives
- Understand Linux user accounts and privilege management
- Explore file permissions and ownership
- Identify running processes and active services
- Reduce attack surface by disabling unnecessary services
- Configure firewall rules using UFW
- Review system logs for security monitoring
- Apply operating system hardening best practices

---

## Environment
- Operating System: Kali Linux
- User Type: Standard user with sudo privileges
- Firewall: UFW (Uncomplicated Firewall)

---

## Task Execution

### 1. User Accounts and Privileges
Commands used:
whoami  
id  

Purpose:
- Identify the current logged-in user
- Understand user ID, group ID, and sudo privileges

---

### 2. File Permissions and Ownership
Commands used:
ls -l  
chmod 640 report.txt  
sudo chown kali:kali report.txt  

Purpose:
- Understand read, write, and execute permissions
- Apply least privilege access to files
- Manage file ownership securely

---

### 3. Running Processes and Services
Commands used:
ps aux | head  
systemctl list-units --type=service --state=running  

Purpose:
- Identify running processes
- List active system services
- Understand how services contribute to the attack surface

---

### 4. Disabling Unnecessary Services
Commands used:
sudo systemctl stop bluetooth  
sudo systemctl disable bluetooth  

Purpose:
- Disable unused services
- Reduce potential attack vectors

---

### 5. Firewall Configuration (UFW)
Commands used:
sudo ufw enable  
sudo ufw status  
sudo ufw default deny incoming  
sudo ufw default allow outgoing  

Purpose:
- Enable firewall protection
- Block unauthorized inbound traffic
- Maintain secure default firewall policies

---

### 6. Log Monitoring
Command used:
cat /var/log/auth.log  

Purpose:
- Review authentication-related activities
- Understand the importance of logs in incident detection

---

### 7. OS Hardening Best Practices
- Use standard user accounts for daily activities
- Apply security updates regularly
- Enable and configure firewall rules
- Disable unnecessary services
- Monitor logs and running processes
- Apply the principle of least privilege

---

## Conclusion
Operating system security is a critical foundation of cybersecurity. By applying proper access controls, managing permissions and services, configuring firewall rules, and monitoring logs, the attack surface of Kali Linux can be significantly reduced.

---

## File Included
OS_Security_Checklist_Task2_Kali.pdf

---
👤 Author
[A.SABARIS]
Cybersecurity Intern

📅 Task Information
Internship: Cybersecurity
Task: Operating System Security Fundamentals (Linux & Windows)
Task Number: 2
