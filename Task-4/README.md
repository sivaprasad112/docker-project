# Task 4 - Secure Monitoring Logs with User Permissions

## 📌 Objective

Secure monitoring logs by allowing access only to a dedicated user.

---

## 👤 Step 1: Create Monitoring User

```bash
sudo useradd monitoruser
sudo passwd monitoruser
```

---

## 📁 Step 2: Create Monitoring Directory

```bash
sudo mkdir -p /opt/container-monitor
```

---

## 🔐 Step 3: Assign Ownership

```bash
sudo chown monitoruser:monitoruser /opt/container-monitor
```

---

## 🔓 Step 4: Set Permissions

```bash
sudo chmod 700 /opt/container-monitor
```

### Explanation:

* Owner → Full access ✅
* Others → No access ❌

---

## 🧪 Step 5: Verify Access Control

### Switch to monitoring user:

```bash
su - monitoruser
cd /opt/container-monitor
```

✔ Access should work

---

### Try with another user:

```bash
su - otheruser
cd /opt/container-monitor
```

❌ Permission denied (Expected)

---

## 📂 Result

* Monitoring user has full access ✅
* Other users are restricted ❌
* Logs are securely stored 🔐

---

## ✅ Conclusion

Successfully implemented secure access control for monitoring logs using Linux user permissions.
