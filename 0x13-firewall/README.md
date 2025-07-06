# 0x13. Firewall

## Description

This project focuses on configuring the `ufw` (Uncomplicated Firewall) tool on an Ubuntu server. The goal is to control incoming and outgoing network traffic by setting up firewall rules.

---

## Task: 0. Block all incoming traffic but...

### Requirements:
- Install and enable `ufw` on `web-01`.
- Block all **incoming** traffic by default.
- Allow only the following **incoming TCP ports**:
  - `22` (SSH)
  - `80` (HTTP)
  - `443` (HTTPS)

---

## UFW Commands Used

```bash
# Allow SSH
sudo ufw allow 22

# Allow HTTP
sudo ufw allow 80

# Allow HTTPS
sudo ufw allow 443

# Deny all other incoming traffic
sudo ufw default deny incoming

# Allow all outgoing traffic (optional but recommended)
sudo ufw default allow outgoing

# Enable UFW
sudo ufw enable

