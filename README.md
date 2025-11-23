# 🖥️ Home Server (Debian) — Self-Hosted Infrastructure

This repository documents my personal **homelab server** running on Debian.  
I use it to host private cloud services, manage my own infrastructure, and practice DevOps fundamentals in a real environment.

---

# 🚀 Running Services

### ☁️ **Nextcloud**
Personal cloud platform  
• Files & storage  
• iPhone sync  
• Web access  
• Hosted at: **https://golden-hub.org**

---

### 📸 **Immich**
High-performance self-hosted photo backup  
• Auto upload from iPhone  
• Local private gallery  
• Runs via Docker

---

### 🔁 **Nginx Reverse Proxy**
Handles:  
• HTTPS  
• routing to services  
• Cloudflare integration

---

### 🔒 **Cloudflare**
Used for:  
• DNS  
• SSL  
• Protection  
• Secure traffic proxy

---

### 📡 **Telegram Monitoring**
Custom Bash-based monitoring:  
• Alerts when services go down  
• Notifies when they recover  
• Daily health report at 07:00  
• CPU / RAM / Disk stats  
• Uptime information  

---

# 🧩 Technologies & Tools

![Linux](https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black)
![Debian](https://img.shields.io/badge/Debian-A81D33?logo=debian&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)
![Compose](https://img.shields.io/badge/Docker_Compose-2496ED?logo=docker&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?logo=nginx&logoColor=white)
![Cloudflare](https://img.shields.io/badge/Cloudflare-F38020?logo=cloudflare&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-121011?logo=gnu-bash&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?logo=git&logoColor=white)
![Networking](https://img.shields.io/badge/Networking-0066CC)

---

# 🗂️ Repository Structure

```
Home-Server-Debian/
├── docker-compose files
├── nginx reverse proxy configs
├── telegram monitor
└── documentation
```

---

# 🏗️ Architecture Overview

```
                    Internet
                        │
                🌐 Cloudflare Proxy
                        │
                ┌───────▼───────┐
                │   Nginx Proxy  │
                └───────┬───────┘
        ┌───────────────┼────────────────┐
        │               │                │
   Nextcloud        Immich       Telegram Monitor
  (Docker)         (Docker)      (Bash + systemd)
```

---

# 🎯 Purpose of This Project

I built this server to:

• learn DevOps basics  
• understand self-hosting  
• practice Docker & networking  
• manage my own infrastructure  
• run real services 24/7  
• gain hands-on Linux experience  

Everything is deployed, configured, and maintained manually on my own hardware.
