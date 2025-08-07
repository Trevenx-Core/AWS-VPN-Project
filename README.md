# Proof of concept DO NOT USE IN PRODUCTION

# AWS VPN Project

## 🔒 Overview
Secure VPN server hosted on AWS EC2 using OpenVPN.

## 🧠 Key Skills Demonstrated
- EC2 provisioning
- Linux/SSH
- OpenVPN configuration
- Network routing
- Secure file transfer

## 🛠️ Tools Used
AWS EC2, Linux, OpenVPN, SCP, SSH

## 📊 Architecture Diagram
<img width="958" height="131" alt="vpn diagram" src="https://github.com/user-attachments/assets/1c5c3f61-1ce9-41d2-af9d-193ed2b24154" />

## 🪜 Setup Steps
1. Launch EC2 instance
2. Configure Security Groups
3. SSH into instance and install OpenVPN
4. Transfer client config file
5. Connect from OpenVPN client

## ✅ Outcome
Functional VPN tunnel from local device to AWS.

## Possible future improvements
Creation of IAM role for EC2 with least privilege
Enable OpenVPN logs and possible implementation of CloudWatch Agent to stream logs
Hardening of network security through EC2 security settings
Certificate based authentication

## Proof of concept DO NOT USE IN PRODUCTION
