# 🔒 AWS VPN Project (Proof of Concept)

> **Note:** This project is for demonstration purposes only — **DO NOT USE IN PRODUCTION.**

---

## 📝 Overview
This project demonstrates deploying a **secure VPN server** on AWS EC2 using **OpenVPN**.  
It follows best practices for secure remote access, encryption, and network routing in the cloud.

---

## 🧠 Key Skills Demonstrated
- **EC2 provisioning** for hosting VPN services
- **Linux server administration** via SSH
- **OpenVPN configuration** for encrypted tunnels
- **Network routing** through a secure tunnel
- **Secure file transfer** for VPN profiles

---

## 🛠 Tools Used
- **AWS EC2**
- **Linux (Ubuntu 22.04)**
- **OpenVPN**
- **SCP / SSH**
- **Security Groups (AWS)**

---

## 🧱 Architecture Diagram
![Architecture Diagram](architecture-diagram.png)

---

## ⚙ Setup Steps
1. **Launch EC2 instance**
   - Choose Ubuntu 22.04 as the OS
   - Assign an Elastic IP (optional)

2. **Configure Security Groups**
   - Allow UDP 1194 (OpenVPN default port)
   - Allow SSH (port 22) from trusted IPs

3. **Install OpenVPN**
   - SSH into the instance  
   - Install OpenVPN and configure the server

4. **Transfer VPN profile**
   - Use `scp` to securely copy `.ovpn` file to local machine

5. **Connect from OpenVPN client**
   - Import `.ovpn` profile into OpenVPN client
   - Verify tunnel connectivity

---

## ✅ Outcome
A functional VPN tunnel from a local device to AWS with:
- **Encrypted traffic** using OpenVPN
- **Secure remote access** via EC2
- **Custom configuration** for routing internet traffic

---

## 🔧 Possible Future Improvements
- **IAM role creation** for EC2 with least privilege
- **Enable OpenVPN logs** and stream them via CloudWatch
- **Harden EC2 security** with stricter Security Group rules
- **Implement certificate-based authentication**
