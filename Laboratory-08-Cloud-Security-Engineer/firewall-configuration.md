# Firewall Configuration

## 1. Allow SSH

```bash
sudo ufw allow ssh
```

This command allows incoming SSH connections on port 22 so administrators can remotely manage the server.

## 2. Configure the Default Deny Policy

```bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
```

These commands block incoming traffic by default while allowing outgoing connections from the server.

## 3. Enable the Firewall

```bash
sudo ufw enable
sudo ufw status verbose
```

These commands enable the firewall and display its current status and default policies.

## 4. Allow Port 8080

```bash
sudo ufw allow 8080/tcp
sudo ufw status numbered
```

These commands allow incoming TCP traffic on port 8080 and display the firewall rules with their numbers.

## 5. SSH Security Precaution

If `sudo ufw enable` is run before `sudo ufw allow ssh`, incoming SSH connections may be blocked, potentially preventing administrators from accessing the server remotely.