#🏠 Home Server (Debian) — Self-Hosted Project

This repository documents my personal home server setup.  
I built and configured this server for learning purposes and to gain hands-on experience with Linux, Docker, networking, and self-hosting.  
During the process I used ChatGPT as a technical assistant, but all setup, troubleshooting, and execution were done by me manually.

---

## 🚀 Project Overview

My home server runs on **Debian** and hosts two main self-hosted services using **Docker Compose**:

### 1️⃣ Nextcloud
- Personal cloud for files  
- Works over HTTPS  
- Connected to a custom domain  
- Accessible from iPhone and PC  
- Stores data locally on the server

### 2️⃣ Immich
- Privacy-focused local photo backup  
- Automatic upload from iPhone  
- Fast indexing and media organization  
- Runs with PostgreSQL and Redis  
- Fully self-hosted on my hardware

---

## 🔧 Technologies Used

- **Debian Linux**
- **Docker & Docker Compose**
- **Nginx reverse proxy**
- **Cloudflare DNS / SSL**
- **Bash scripting**
- **Systemd services**
- **Firewall hardening (Fail2Ban / ufw)**

I configured each service by editing Docker Compose files, setting up Nginx proxy rules, managing DNS records, fixing errors, and monitoring logs.

---

## 📡 Monitoring & Automation

I also created a small monitoring script that sends Telegram notifications, including:

- Service status (Nextcloud / Immich)
- Alerts when a service is down
- Daily server health report at 07:00:
  - uptime  
  - CPU usage  
  - RAM usage  
  - disk usage  
  - HTTP status of each service  

---

## 🔐 Security Setup

- Cloudflare proxy & SSL  
- Limited SSH access  
- Private local network  
- Docker container isolation  
- Fail2Ban for brute-force protection  
- Regular updates and logs monitoring  

---

## 🎯 Purpose of This Project

The goal of this project is to:

- Learn Linux administration  
- Practice Docker-based deployments  
- Understand domains, DNS, and reverse proxying  
- Maintain real services running 24/7  
- Gain practical experience useful for DevOps and system administration  

This project represents real-world hands-on practice on my own hardware.
