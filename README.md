# 🔐 Create a New Linux User & Add to Sudoers 🧑‍💻

**creating a new user and adding them to the sudoers file**! 🚀  
## 🧩 Step 1: Create a New User

Use the following command to create a new user:
```bash
sudo adduser devopsuser
# 🔐 Create a New Linux User & Add to Sudoers 🧑‍💻

Hey everyone 👋  

Today I explored one of the most essential Linux administration tasks —  
**creating a new user and adding them to the sudoers file**! 🚀  

This is a key skill for anyone learning **Linux, DevOps, or Cloud Administration.**  

---

## 🧩 Step 1: Create a New User

Use the following command to create a new user:
```bash
sudo adduser devopsuser


🔒 Step 3: (Optional) Allow Sudo Access Without Password

If you want to allow the user to use sudo without being prompted for a password (use carefully ⚠️):

Open the sudoers file:

sudo visudo


Add this line at the end:

devopsuser ALL=(ALL:ALL) NOPASSWD:ALL
Save and exit using:

Ctrl + X → Y → Enter

🧠 Step 4: Verify Access

Switch to the new user:

su - devopsuser


Then check sudo access:

sudo whoami
