# Task 5 - UFW Firewall Configuration

## 📌 Objective
To secure the server using UFW (Uncomplicated Firewall).

## 🔧 Commands Executed

sudo ufw enable
sudo ufw status numbered
sudo ufw delete 1
sudo ufw delete 2
sudo ufw allow from 13.207.4.89 to any port 22
sudo ufw allow 80
sudo ufw allow 8000

## ⚙️ Configuration Steps

1. Enabled UFW firewall
2. Removed default SSH access from anywhere
3. Allowed SSH access only from my IP (13.207.4.89)
4. Opened port 80 for web traffic
5. Opened port 8000 for application
6. Verified rules using `ufw status`

## 🔐 Result

- SSH access restricted to specific IP
- Public access allowed for HTTP (80) and app port (8000)
- Server secured successfully

## 📄 Files Used

No additional files used
