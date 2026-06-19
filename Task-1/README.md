# Task 1 - Server Setup and SSH Configuration

## 📌 Objective

Provision a Linux server and configure secure SSH access using key-based authentication.

---

## 🖥️ Environment

* OS: Ubuntu (Virtual Machine)

---

## ⚙️ Steps Performed

### 1. Update System

sudo apt update
sudo apt upgrade -y

---

### 2. Install SSH

sudo apt install openssh-server -y
sudo systemctl start ssh
sudo systemctl enable ssh

---

### 3. Check SSH Status

sudo systemctl status ssh

---

### 4. Find IP Address

ip a

---

### 5. Connect via SSH (Password)

ssh username@server_ip

---

### 6. Generate SSH Key

ssh-keygen

---

### 7. Copy Key to Server

ssh-copy-id username@server_ip

---

### 8. Login Without Password

ssh username@server_ip

---

### 9. Disable Password Login (Security)

sudo nano /etc/ssh/sshd_config

Change:
PasswordAuthentication no

Restart:
sudo systemctl restart ssh

---

## 🔐 Security Features

* SSH enabled
* Key-based authentication configured
* Password login disabled

---

## 📂 Files Used

* ~/.ssh/id_rsa
* ~/.ssh/id_rsa.pub
* /etc/ssh/sshd_config

---

## ✅ Expected Outcome

Secure SSH login without password using SSH keys.

