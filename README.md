# 👾 Lithium V 1.0

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/) ![Language](https://img.shields.io/badge/Language-Bash-Bash) ![Version](https://img.shields.io/badge/Version-1.0-1) ![Tool Type](https://img.shields.io/badge/Tool%20type-Automation-e) ![Open Source](https://img.shields.io/badge/Open%20Source-Yes-g)

A [Beef-XSS](https://github.com/beefproject/beef) web-based automation tool for controlled lab environments.

## ⚠️ DISCLAIMER

This tool is intended for **educational purposes only** and must be used exclusively in **authorized and controlled environments**. 
Do not use it against systems you do not own or do not have explicit permission to test.
The objective of Lithium is to automate a setup process, not to harm any system or network.
The author is not responsible for any misuse, damage, or illegal activity caused by this tool.


## 🛠️ Tool Description

Lithium is a Beef-XSS automation tool for controlled lab environments. Its purpose is to automate the following task: hosting a hook url using a tunneling service.
It provides four options:

- Install Ngrok: Automatically installs ngrok from its official repository, simplifying tunneling setup.
- Enable Ngrok authtoken: Lets the user input and register their ngrok authentication token to enable secure tunneling.
- Start the Testing Environment
- Exit from the tool

Lithium Sets up:
- BeEF login credentials
- Network and hooking parameters
- Public-facing server configuration
- Launches the BeEF framework ready for use

### Hosting the URL
-  Choose the third option on the menu
-  Open a second terminal and start the ngrok tunnel on port 3000(Beef-XSS runs on port 3000):
 
```bash
ngrok http 3000
```
- Lithium will now ask you to insert the NGROK URL: insert it without "https://", otherwise it won't work and you will encounter in an error.
 
- Everything is ready, just wait for the tool to give you the new link. Example output:
 
```
[+] Panel URL: https://bb99-93-37-181-18.ngrok-free.app/ui/panel
[+] Hook URL: https://bb99-93-37-181-18.ngrok-free.app/demos/basic.html
```

# 🪐 OS/Device Compatibility 

| OS/Device                | Is compatible |
|--------                  |----------     |
| iPhone                   | No            |
| Android(Termux)          | Yes           |
| Windows                  | No            |
| Arch Linux               | Yes           |
| Mac OS                   | No            |
| Debian(Kali, Parrot, etc)| Yes           |

## 📝 Prerequisites
- Beef-XSS [Browser Exploitation Framework]
- NGROK [For tunneling]
- NGROK Authtoken
- git [To clone this repository]
- chmod [To make the bash script executable]
- Root
- Any Linux-based operating system


## 💎 Getting started

Clone the repository:

```bash
git clone https://github.com/Zerium-99/Lithium.git
```

Navigate to the "Lithium" folder

```bash
cd Lithium
```

Make the file executable
```bash
chmod +x Lithium.sh
```
Move Lithium.sh to the path where beef-xss is installed.

```bash
mv Lithium.sh <path>
```

Execute the file 

```bash
sudo ./Lithium.sh
```

## 🎯 Use Case

Lithium is designed for:
- Red Team practice
- XSS exploitation labs
- Browser exploitation simulations
- Educational cybersecurity environments

## 📸 Screenshots
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/84e189a4-e837-4c78-98f7-95be1ba2cc44" />







