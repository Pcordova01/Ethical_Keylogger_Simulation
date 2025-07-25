# 🐍 Ethical Keylogger Simulation

### ** Disclaimer: This project is for ethical purposes only!! Please do not be irresponsible!!! **

## 📜 Objective

The purpose of this project is to simulate a credential harvesting technique using a simple Python-based keylogger. It captures keystrokes using the `pynput` library and sends the recorded input to a specified email address after every 10 keystrokes. This simulation offers hands-on insight into common red team tactics such as data exfiltration and credential theft, while also highlighting potential blue team detection strategies—such as monitoring for unusual SMTP activity or unauthorized keylogging behavior. I took inspiration from multiple python-based keyloggers I found on stack overflow, github, and youtube.

## 🔧 Tools Used

- **Python 3**
- **pynput** – for capturing keyboard input
- **smtplib (SMTP with TLS)** – for sending data via Gmail
- **VS Code** – development environment
- **Git & GitHub** – version control and documentation

## 🧠 Skills Learned

- Keylogging mechanisms and input capture
- Secure email transmission using **SMTP** with **TLS**
- Simulating basic exfiltration techniques
- Mapping behavior to **MITRE ATT&CK** techniques
- Implementing ethical hacking projects responsibly
- Writing maintainable, modular Python code
- Basic red team methodology and blue team awareness

## ✅ Features

- Captures all keystrokes typed on the keyboard
- Sends logged keystrokes to a Gmail inbox every 10 characters
- Uses TLS encryption for secure data transmission
- Modular script separation for email and logging logic
  
## 📽️ Video Demonstration
<video src="https://github.com/user-attachments/assets/e71172f6-4e8d-4a28-bc02-c7f5f5341897" controls width="200"></video>

## 🔍 Detection Considerations
- **Monitor SMTP Traffic**- Look for unusual email activity from non-email related apps.
- **Excessive Background Processes**- Keyloggers usually run in the background. Try spotting unusual processes running without windows.
- **Frequent Outbound Emails**- Watch out for small, repeated emails that suggest data exfiltration.
  
## ⚙️ How to Run the App

- Clone the repository: [https://github.com/your-username/python-keylogger-email-demo.git  ](https://github.com/Pcordova01/python-keylogger-emailer/blob/main/README.md)
- Open the project folder in VS Code
- - Open a terminal and run the following to install pynput:
  ```bash
  pip install pynput
- Open the `send_email.py` file and replace the email, password, and receiver with your own Gmail and App Password
- Run 'keylogger.py' and track your keys!!
