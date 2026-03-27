# 📸 CamPhish (Educational Fork)

> ⚠️ **Disclaimer:** This project is intended strictly for **educational and ethical cybersecurity testing purposes**. Do NOT use it on any individual or system without **explicit permission**.

---

## Overview

# CamPhish
Grab cam shots from target's phone front camera or PC webcam and location access just sending a link .

# What is CamPhish?
<p>CamPhish is techniques to take cam shots of target's phone front camera or PC webcam. CamPhish Hosts a fake website on in built PHP server and uses ngrok & CloudFlare Tunnel to generate a link which we will forward to the target, which can be used on over internet. website asks for camera permission and location permission and if the target allows it, this tool grab camshots of target's device or easy one out if your browser has already allowd camera and location access to everyone

This fork is maintained for:

* Learning **web security concepts**
* Understanding **client-side permissions**
* Practicing **ethical penetration testing in controlled environments**

---

## 🧠 Key Learning Concepts

* Social Engineering Attacks
* Browser Permission Model (Camera, Location)
* HTTP Tunneling (Cloudflare / Ngrok)
* Client-side Data Capture
* Ethical Hacking Practices

---

## ⚙️ Features

* 📸 Capture camera images (with permission)
* 📍 Capture approximate location data
* 🌐 IP logging
* 🔗 Public link generation using tunneling
* 🎭 Multiple webpage templates

  ---
  A GPS location capture feature has been added.</p>

## Features
<p>In this tool I added two automatic webpage templates for engaged target on webpage to get more picture of cam</p>
<ul>
  <li>Festival Wishing</li>
  <li>Live YouTube TV</li>
  <li>Online Meeting [Beta]</li>
  <li>GPS Location Tracking</li>
</ul>
<p>A cleanup script has been added to remove all unnecessary files and logs.</p>

## This Tool Tested On :
<ul>
  <li>Kali Linux</li>
  <li>Termux</li>
  <li>MacOS</li>
  <li>Ubuntu</li>
  <li>Parrot Sec OS</li>
  <li>Windows (WSL)</li>
</ul>

<p>The cam files and saved location will also be removed.</p>

## Change Log:

<p><b>Version: 2.0:</b> Added GPS Location Tracking</p>
<ul>
  <li>Added: GPS location capturing functionality</li>
  <li>Added: Google Maps integration for captured locations</li>
  <li>Added: Location accuracy reporting</li>
  <li>Added: Improved loading screen with location request</li>
</ul>

---

## 🛠️ Installation (Kali Linux)

```bash
sudo apt update && sudo apt upgrade -y
sudo apt install git php curl wget unzip -y
```

---

## 📥 Setup

```bash
git clone https://github.com/YOUR_USERNAME/CamPhish.git
cd CamPhish
chmod +x camphish.sh
```

---

## ▶️ Usage

```bash
bash camphish.sh
```

### Steps:

1. Select a template
2. Choose tunnel method:

   * Cloudflared (recommended)
   * Ngrok
3. A public URL will be generated

---

## 🌐 Tunnel Options

### 🔹 Cloudflared (Recommended)

* No login required
* Faster setup
* More reliable for testing

### 🔹 Ngrok

* Requires account and auth token
* Useful for advanced configurations

---

## 📁 Output Files

After successful testing:

| File/Folder        | Description      |
| ------------------ | ---------------- |
| `cam*.png`         | Captured images  |
| `location_*.txt`   | Location data    |
| `saved.ip.txt`     | IP logs          |
| `saved_locations/` | Location storage |
| `*.log`            | Debug logs       |

---

## 🧪 Testing Guidelines

✅ Allowed:

* Your own device
* Virtual machines
* Lab environments

❌ NOT allowed:

* Sending links to real users without consent
* Any unauthorized surveillance
* Malicious usage

---

## 🧹 Cleanup (Important)

Remove all collected data after testing:

```bash
rm -rf cam*.png location_*.txt saved* *.log
```

OR

```bash
bash cleanup.sh
```
OR

```bash
rm cam*.png
rm location_*.txt
rm saved.ip.txt saved.locations.txt
rm -rf saved_locations
rm *.log
```
---

## ⚠️ Limitations

* Requires **user permission** (camera/location)
* Modern browsers may block requests
* Not effective without user interaction

---

## 🔐 Ethical Use Policy

This project must be used only for:

* Cybersecurity education
* Awareness demonstrations
* Personal lab experimentation

Any misuse is strictly discouraged and may be illegal.

---

## 🧩 Future Improvements (Ideas)

* Add secure logging mechanism
* Integrate with SIEM tools
* Improve UI templates
* Add permission simulation dashboard

---

## 📚 Recommended Learning Path

* OWASP Top 10
* Web Security Testing
* DevSecOps Practices
* Network Security Basics

---

## 🤝 Contribution

Contributions are welcome!
Feel free to fork, improve, and submit pull requests.

---

## 📜 License

This project follows the original repository’s license.

---

## ⭐ Acknowledgment

Original project by:
👉 https://github.com/techchipnet/CamPhish
Edited and Used by:
@PriyanshuSingh10114
---

## 🙌 Final Note

> “Learn ethically. Build responsibly. Secure everything.”

---

### Important Notice
Unauthorized reuploading of this project is prohibited.
