# 📂 Lab: File Share with NTFS and Share Permissions

Learn how to securely share a folder using NTFS and Share permissions in Windows. This setup is useful for system administrators, lab builders, and anyone learning Windows Server/File Services.

---

## 🧰 Tools Used

- Windows Server or Windows 10/11 Pro
- Active Directory (optional)
- File Explorer (GUI)
- Command Prompt (CMD)

---

## 🪜 Step-by-Step Guide

### ✅ Step 1: Create a Shared Folder

1. Go to File Explorer
2. Navigate to `C:\` or `D:\`
3. Create a folder:

![imagealt](https://github.com/techtracker619/serverfiles/blob/b2ed30ff913c89793a1a5eabddcb5896c415fecf/screenshots/VirtualBox_AC-DC-SERVER_27_06_2025_18_23_28.png)


---

### 🔐 Step 2: Set NTFS Permissions

1. Right-click folder > `Properties`
2. Go to **Security** tab
3. Click **Edit** > **Add** group or user
4. Grant permissions:
- Read
- Modify
- Full Control

📸 Screenshot:  
![NTFS Permissions](./screenshots/02-ntfs-permissions.png)

---

### 🌐 Step 3: Share the Folder

1. Click **Sharing** tab
2. Click **Advanced Sharing**
3. Check ✔️ “Share this folder”
4. Set share name
5. Click **Permissions**
6. Grant share-level permissions

📸 Screenshots:  
- ![Share Tab](./screenshots/03-share-tab-settings.png)  
- ![Share Permissions](./screenshots/04-share-permissions.png)

---

### 💻 Step 4: Access the Share Remotely

On a client machine, press `Windows + R` and enter:

```cmd
\\SERVER-NAME\SharedDocs
