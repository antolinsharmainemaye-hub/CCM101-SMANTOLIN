# Laboratory 08 - Cloud Security Engineer

## Mission Overview

This mission focuses on securing an Ubuntu server using the UFW host-based firewall. It involves auditing network access, applying a Default Deny policy, and allowing only the required services for SSH administration and web application access.

## Objectives

- Understand the Principle of Least Privilege and Attack Surface.
- Audit and manage open network ports.
- Configure UFW with a Default Deny incoming policy.
- Allow SSH traffic on port 22.
- Allow web application traffic on TCP port 8080.
- Verify firewall rules and test web application access.
- Document firewall configurations and security practices.

## Commands Executed

| Command | Purpose |
|---|---|
| `docker run -d -p 8080:80 --name secure-web-app nginx` | Deploys an Nginx container on port 8080. |
| `curl http://localhost:8080` | Tests the web application response. |
| `sudo ufw allow ssh` | Allows incoming SSH connections. |
| `sudo ufw default deny incoming` | Blocks incoming traffic by default. |
| `sudo ufw default allow outgoing` | Allows outgoing traffic by default. |
| `sudo ufw enable` | Enables the firewall. |
| `sudo ufw status verbose` | Displays firewall status and default policies. |
| `sudo ufw allow 8080/tcp` | Allows incoming TCP traffic on port 8080. |
| `sudo ufw status numbered` | Displays firewall rules with their numbers. |

## Skills Learned

- Applying basic cloud security principles.
- Configuring a host-based firewall using UFW.
- Implementing a Default Deny incoming policy.
- Managing SSH and web application port access.
- Testing application connectivity with `curl`.
- Documenting security configurations and maintaining a GitHub portfolio.