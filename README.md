# NovaShyld Task_1 – Foundations of Ethical Hacking & Penetration Testing

## 📌 Objective

The objective of this task was to build a strong foundation in ethical hacking and penetration testing by understanding the professional methodology, legal boundaries, lab setup, Linux basics, networking essentials, reconnaissance, scanning, and vulnerability assessment in a controlled environment.

---

## 🛠️ Tools & Platforms Used

* Oracle VM VirtualBox
* Kali Linux (Attacker Machine)
* Metasploitable2 (Target Machine)
* Nmap
* Metasploit Framework
* Telnet
* FTP
* Netcat
* Web Browser

---

## ⚙️ Lab Environment Setup

A secure virtual lab was created using Oracle VM VirtualBox.

* Kali Linux was configured as the attacker machine.
* Metasploitable2 was configured as the vulnerable target machine.
* NAT + Host-Only Adapter networking was used.
* Manual IP assignment and DHCP verification were performed.

Assigned IP Addresses:

* Kali Linux: 192.168.56.101
* Metasploitable2: 192.168.56.102

This ensured both machines were isolated in a safe penetration testing environment.

---

## 🐧 Linux Essentials Practiced

Basic Linux commands were tested to understand navigation and system interaction:

* pwd
* ls
* cd
* chmod
* apt update
* ifconfig / ip a

These commands helped in learning file handling, package updates, and interface identification.

---

## 🌐 Networking Fundamentals Verified

The following networking fundamentals were practiced:

* IP Address identification
* Host communication testing
* Port/service visibility
* Protocol exposure

Commands used:

* ping
* traceroute
* ss -tuln

---

## 🔍 Reconnaissance & Scanning Performed

### 1. Connectivity Test

Successful ICMP communication was established between Kali Linux and Metasploitable2 using ping.

### 2. Nmap Service Version Scan

Nmap -sV scan was used to enumerate open ports and running services.
Open services identified included:

* FTP (21)
* SSH (22)
* Telnet (23)
* SMTP (25)
* HTTP (80)
* NetBIOS (139)
* SMB (445)

### 3. Vulnerability NSE Scan

Nmap vulnerability scripts were executed using:
`nmap --script vuln 192.168.56.102`
This helped identify insecure and exploitable services.

---

## 💥 Exploitation & Unauthorized Access Demonstration

### Telnet Weak Credential Access

Default credentials were used to gain unauthorized Telnet access to the target machine.

### FTP Weak Access Verification

FTP service was tested and directory listing was successfully performed.

### Banner Grabbing

Netcat was used to grab banners from exposed services to verify service disclosure.

### Web Service Exposure

The hosted Metasploitable vulnerable web applications were accessed through browser verification.

---

## 📸 Evidence Collected

A total of 9 practical screenshots were captured as proof:
1. Metasploitable Network Settings
2. Kali Linux Network Settings
3. Ping Connectivity Test
4. Nmap Service Scan
5. Metasploit Framework Initialization
6. Telnet Unauthorized Login
7. Shell Access Verification
8. FTP Access Proof
9. Vulnerable Web Page Access
10. Banner Grabbing
11. Nmap Vulnerability NSE Scan

---

## 📊 Key Findings

* The target machine exposed multiple insecure services.
* Weak/default credentials allowed unauthorized access.
* FTP and Telnet services were insecurely configured.
* Vulnerability scripts highlighted exploitable weaknesses.
* The lab successfully demonstrated the Recon → Scan → Exploit → Report methodology.

---

## ✅ Conclusion

Task 1 successfully established the practical foundation of ethical hacking and penetration testing. A controlled virtual lab was created, reconnaissance and scanning were performed, insecure services were identified, and unauthorized access was demonstrated in a safe environment. This task provided hands-on understanding of professional pentesting workflow and cybersecurity fundamentals.

---

## 🔗 Repository Contents

This repository contains:

* Screenshots Folder
* Mini Report
* Required Practical Notes
* Walkthrough Video Link (For LinkedIn Submission)

---

## 👨‍💻 Submitted For

NovaShyld Technologies Internship Program
