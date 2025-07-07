# 🛠️ Day 0 – Lab Setup & Preparation

**Date:** July 7, 2025  
**Objective:** Set up a secure and isolated ethical hacking lab environment for all future practical tasks.

---

## ✅ Completed Tasks:

### 1. 💻 Kali Linux Installation
- Installed Kali Linux using VirtualBox.
- Configuration:
  - **RAM:** 4GB
  - **Storage:** 30GB virtual HDD
  - **Networking:** NAT (Internet access inside VM)
- Updated Kali system packages:
  ```bash
  sudo apt update && sudo apt upgrade -y
  ```

---

### 2. 🐳 Installed Docker in Kali Linux
Docker allows running isolated containers for tools and vulnerable environments.

**Commands Used:**
```bash
sudo apt install docker.io -y
sudo systemctl start docker
sudo systemctl enable docker
```

---

### 3. 📦 Pulled & Ran DVWA Container
**DVWA** (Damn Vulnerable Web Application) helps practice real-world web vulnerabilities safely.

**Commands Used:**
```bash
sudo docker pull vulnerables/web-dvwa
sudo docker run -d -p 80:80 vulnerables/web-dvwa
```

- Confirmed that container is running using:
  ```bash
  sudo docker ps
  ```

---

### 4. 🌐 Accessed DVWA Interface
- Opened browser in Kali VM
- Visited `http://localhost/`
- Logged in with:
  - **Username:** `admin`
  - **Password:** `password`
- Clicked on **"Create / Reset Database"** to initialize DVWA
- Set **Security Level** to **Low** from the settings tab

---

### 5. 🔍 Verified DVWA Functionality
- Navigated to:
  - **SQL Injection**
  - **XSS (Reflected)**
  - **File Upload**
- Confirmed DVWA is ready for exploitation practice

---

## 🧰 Tools Installed Today:

| Tool         | Purpose                            |
|--------------|-------------------------------------|
| Kali Linux   | OS for ethical hacking              |
| Docker       | Containerized vulnerable apps       |
| DVWA         | Web vulnerability practice target   |

---

## 🔗 References:
- [DVWA GitHub](https://github.com/digininja/DVWA)
- [Kali Linux Official Site](https://www.kali.org/get-kali/)
- [TryHackMe DVWA Room](https://tryhackme.com/room/dvwa)

---

## 📝 Notes:
- All setup is complete and working as expected.
- Will begin Day 1 with **Networking Basics, OSI/TCP-IP Models, and Wireshark**.
- All progress will be documented in this repo under respective weeks.

---

## 🚀 Next:
[→ Proceed to Day-1.md](./Day-1.md)
