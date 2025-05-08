# 🚀 Kubernetes WordPress-MySQL Deployment with Secrets & RBAC

This project demonstrates a **secure, multi-tier application deployment** on **Kubernetes** using **WordPress** as the frontend and **MySQL** as the backend. It includes secure password handling using **Kubernetes Secrets**, access control via **RBAC**, and a default **rolling update strategy** for seamless updates.

---

## 📦 Features

- ✅ Multi-tier architecture with WordPress & MySQL
- 🔐 Secure password management with Kubernetes Secrets
- 👤 Role-Based Access Control (RBAC) for restricted access
- 📦 ClusterIP for internal database communication
- ♻️ Rolling Update strategy (default in Kubernetes)
- 🛠 Dry-run & YAML generation for manifest clarity

---

## 🧪 Setup Instructions

### 1. **Create a Kubernetes Secret**
--> kubectl create secret generic mysql-pass --from-literal=password=YOUR_PASSWORD



💡 Helpful Commands
Command	    Purpose
kubectl   apply -f file.yaml	Deploy resources
kubectl   get all	View all deployed resources
kubectl   describe secret mysql-pass -o yaml	Check encoded password
`echo    'base64string'	openssl base64 -d`
kubectl   create deployment --image=image-name --dry-run=client -o yaml > file.yaml	Generate YAML

📝 Summary
1. Deployed a secure, scalable WordPress-MySQL application on Kubernetes.

2. Passwords managed with Secrets and encoded with base64.

3. Access to Secrets limited using RBAC.

4. Used --dry-run -o yaml for clean configuration generation.

✅ Conclusion
This project highlights the best practices in deploying cloud-native applications securely using Kubernetes. From handling sensitive data with Secrets to applying RBAC and ensuring internal-only access with ClusterIP, it reinforces how modern DevOps workflows manage complexity, security, and collaboration.


🙌 Credits
Developed Tejaswi Pathak

## **For Reference i have added Security-Multi.pdf file for better understanding and it also include output images** ##
