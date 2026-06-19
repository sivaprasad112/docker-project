# Task 5 - Firewall Configuration (UFW)

## 📌 Objective
Secure server by restricting SSH access.

## 🔧 Commands Executed

sudo ufw enable
sudo ufw status numbered
sudo ufw delete 1
sudo ufw delete 2
sudo ufw allow from 13.207.4.89 to any port 22
sudo ufw allow 80
sudo ufw allow 8000

## 🔐 Result

- SSH restricted to specific IP
- Ports 80 and 8000 open
