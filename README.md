# Linux User & Sudoers Setup Guide | Jenkins Setup



🔐 Create a New Linux User & Add to Sudoers 🧑‍💻

Hey everyone 👋  

Today I explored one of the most essential Linux administration tasks —  
**creating a new user and adding them to the sudoers file**! 🚀  

This is a key skill for anyone learning **Linux, DevOps, or Cloud Administration.**  

---

## 🧩 Step 1: Create a New User

Use the following command to create a new user:

```bash
sudo adduser devopsuser

```


⚙️ Step 2: Add User to the Sudo Group

Once the user is created, give them admin privileges using:

```bash
sudo usermod -aG sudo devopsuser

```

✅ This allows the user to execute commands with sudo.



Switch to the new user:

```bash
su  - devopsuser

``` 



🔒 Step 3: Allow Sudo Access Without Password

If you want to allow the user to use sudo without being prompted for a password (use carefully ⚠️):

Open the sudoers file:

```bash
sudo nano /etc/sudoers

```
 Add this line at the end:
 
```bash
devopsuser ALL=(ALL:ALL) NOPASSWD:ALL
```
Save and exit using:
```bash
Ctrl + X → Y → Enter
```

add script in jenkins here i made simple .sh fir testing
```
sudo mkdir /home/bhushan/data
```

⚡ Pro Tip

Always use sudo responsibly.
Granting passwordless sudo access can be risky — use it only when necessary in trusted environments.


👨‍💻 Author

Shivam Garud
📍Devops & Cloud engineer

🔗 Connect with me on LinkedIn

## 🔗 Links

[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/shivam-garud-371b5a307/)
[![Medium](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://medium.com/@shivam.garud2011/)

