# Task 5 - Firewall Configuration (UFW)

## 🔧 Commands Executed

sudo ufw enable
sudo ufw status numbered
sudo ufw delete 1
sudo ufw delete 2
sudo ufw allow from 13.207.4.89 to any port 22
sudo ufw allow 80
sudo ufw allow 8000

## ⚙️ Configuration Steps

1. Installed and enabled UFW firewall
2. Allowed SSH access only from my IP address (13.207.4.89)
3. Removed default SSH access from anywhere
4. Allowed HTTP traffic on port 80
5. Allowed application traffic on port 8000
6. Verified firewall rules using `ufw status`

## 📄 Files Used

No additional files were used in this task.
