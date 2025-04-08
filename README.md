# Launch-and-Connect-to-a-Windows-EC2-Instance-on-AWS-Free-Tier-
This project demonstrates how to launch a Windows Server EC2 instance on AWS Free Tier, retrieve the administrator credentials, and connect securely using Remote Desktop Protocol (RDP). It includes step-by-step documentation and visuals, making it a beginner-friendly walkthrough for deploying and accessing a cloud-based Windows server.
# 🖥️ Launch and Connect to a Windows EC2 Instance on AWS (Free Tier)

## 📌 Overview

This project demonstrates how to launch a **Windows EC2 instance** on **Amazon Web Services (AWS)** and connect to it using **Remote Desktop Protocol (RDP)**. It’s part of my hands-on AWS learning journey and serves as a public portfolio project for future employers.

---

## 🛠️ Tools & Technologies Used

- **Amazon EC2 (Elastic Compute Cloud)**
- **Windows Server 2019 Base**
- **RDP (Remote Desktop Protocol)**
- **AWS Key Pair (.pem)**
- **Git & GitHub**
- **Remote Desktop Connection (Windows/macOS)**

---

## ✅ Project Goals

- [x] Launch a free-tier Windows Server EC2 instance  
- [x] Generate and decrypt the admin password  
- [x] Connect via RDP securely  
- [x] Document the entire process with visuals  
- [x] Upload project to GitHub

---

## 🧭 Step-by-Step Process

### 🖱️ 1. Launch the EC2 Instance

- Selected **Windows Server 2019 Base (Free Tier eligible)**
- Chose instance type **t2.micro**
- Created a new **key pair** named `windows-keypair.pem`
- Configured **security group** to allow **RDP (port 3389)** only from **my IP**
- Launched the instance

📸 _Screenshot: Instance launched successfully_  
![EC2 Launch](images/ec2-launch.png)

---

### 🔑 2. Retrieve Administrator Password

- Waited ~4 minutes for the instance to initialize
- Navigated to **Connect > RDP Client > Get Password**
- Uploaded `.pem` file to decrypt the password

📸 _Screenshot: Decrypted password in AWS console_  
![Decrypt Password](images/decrypt-password.png)

---

### 💻 3. Connect via Remote Desktop

- Opened **Remote Desktop Connection**
- Entered **public IPv4 address** of instance
- Used `Administrator` and decrypted password to log in
- Accepted the certificate warning

📸 _Screenshot: Successful RDP connection_  
![RDP](images/rdp-connected.png)

---

## 📁 Project Structure

