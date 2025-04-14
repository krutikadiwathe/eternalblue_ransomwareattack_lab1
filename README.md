# 🔐 Cybersecurity Lab 1 – EternalBlue Exploit, OSINT, and Vulnerability Scanning

**Course:** CIS 675 - Information Security  
**Instructor:** Sathish Kumar  
**Student:** Krutika Bhushan Diwathe  
**Semester:** Spring 2025  
**Institution:** Cleveland State University  

---

## 🧠 Overview

This lab demonstrates advanced cybersecurity techniques through a simulated attack and defense scenario. The primary focus areas include:

- **EternalBlue Exploit Simulation** (MS17-010)
- **Open Source Intelligence (OSINT) Reconnaissance**
- **Vulnerability Scanning using SPARTA and Nmap**
- **Exploit Deployment using Metasploit**
- **Ransomware Execution & Decryption Process**

All experiments were conducted in a controlled sandbox environment provided by the Ohio Cyber Range Infrastructure (OCRI).

---

## 📚 Lab Modules

### 🔸 Module 1: EternalBlue Ransomware Attack Scenario
- Target: Windows 7 SP1 (vulnerable SMBv1)
- Exploit: MS17-010 using `exploit/windows/smb/ms17_010_eternalblue`
- Tools: Kali Linux, Metasploit
- Payloads: Ransomware executable (`game.exe`) and decryption tool (`decryptor.exe`)
- Outcome:
  - Gained Meterpreter session access
  - Deployed ransomware
  - Encrypted victim files
  - Decryption process executed after payload delivery

📸 Screenshots:
- Ransomware file extraction in Kali Linux  
- Successful Meterpreter session (WIN)  
- "You Are Hacked" screen message  
- Encrypted and then decrypted files

---

### 🔸 Module 2: OSINT Tools Exploration
- Reconnaissance on `nmap.org` using:
  - `whois`
  - Google Dorks: `site:.gov inurl:reset ext:docx inbody:password`
  - Shodan (searching Ubuntu servers on port 22 in Cincinnati, OH)
  - DNS enumeration tools: `Sublist3r`, `Fierce`, `Spiderfoot`
- Active Recon:
  - Performed port scans using Nmap on `scanme.nmap.org`
  - Used Nmap NSE scripts (`http-enum`, `smb-enum-users`, `nfs-ls`, etc.)

💡 Key Outputs:
- Discovered Apache & OpenSSH versions
- Enumerated DNS, NFS, Samba services
- Extracted sensitive metadata and directory listings

---

### 🔸 Module 3: Vulnerability Scanning with SPARTA
- Network Scope: `192.168.2.0/24`
- Scanning Target: Metasploitable2 and Windows XP
- Discovered:
  - 15+ open services on Metasploitable (e.g., FTP, VNC, PostgreSQL)
  - EternalBlue vulnerability on Windows XP (port 445)

🛠 Tools: SPARTA GUI, Nmap with version and OS detection, Metasploit

📌 Vulnerabilities Identified:
- Remote code execution (RCE)
- Unauthenticated access to bind shells and database servers
- NFS share access without authentication

---

## 🧪 Skills Demonstrated

- 🔧 Vulnerability Assessment & Penetration Testing
- 🧩 Exploit Development with Metasploit
- 🕵️ OSINT & Passive Reconnaissance
- 🌐 Network Scanning and Port Enumeration
- 🔒 Ethical Hacking and Secure Configuration Analysis
- 💬 Risk Mitigation Planning

---

## 🛡️ Countermeasures and Mitigations

- Apply security patches regularly (especially **MS17-010**)
- Disable legacy protocols (SMBv1)
- Enable host-based firewalls and block unused ports (like 445)
- Enforce strong password policies and MFA
- Conduct regular vulnerability scans and user awareness training
- Maintain offline backups and endpoint detection tools

---

## ⚠️ Legal Disclaimer

> This lab was conducted strictly in a **virtualized sandbox environment** designed for educational purposes.  
> Attempting these techniques on unauthorized systems is illegal and unethical.

---

## 📌 About Me

**Krutika Bhushan Diwathe**  
💻 Master’s in Computer Science – Cleveland State University  
🎯 Aspiring Cybersecurity Engineer | Ethical Hacker | Security Analyst  
🌐 [LinkedIn](https://www.linkedin.com/in/krutika-diwathe) | 📫 [Email](mailto:krutika.diwathe16@gmail.com)

