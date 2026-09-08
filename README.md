<div align="center">

# 🛡️ CYBERSTER Internship - Red Team (Offensive Security) Track
### *12-Week Intensive Practical Roadmap & Task Repository*

[![Status](https://img.shields.io/badge/Status-Completed%20%2F%20Active-success?style=for-the-badge&logo=git&logoColor=white)]()
[![Track](https://img.shields.io/badge/Track-Red%20Team%20%7C%20Offensive%20Security-red?style=for-the-badge&logo=kalilinux&logoColor=white)]()
[![Author](https://img.shields.io/badge/Maintained%20by-Daniyal%20Shahid-blue?style=for-the-badge&logo=github&logoColor=white)]()
[![Batch](https://img.shields.io/badge/CYBERSTER-Batch%202-orange?style=for-the-badge)]()

<p align="center">
  <img src="https://media.giphy.com/media/3oKIPnAiaMCws8nOsE/giphy.gif" width="600px" alt="Hacker Animation"/>
</p>

*“Offensive security is not just about breaking systems; it's about understanding how they fail so we can build them stronger.”*

</div>

---

## 👨‍💻 Author & Maintainer
This repository is meticulously documented, structured, and maintained by **Daniyal Shahid** as part of the **CYBERSTER Internship Batch 2 (Red Team Track)**. It serves as an official log of all weekly tasks, exploit scripts, lab notes, and professional penetration testing deliverables.

---

## 🧭 Program Philosophy & Execution Model
Instead of passive classroom learning, this 12-week internship follows an action-oriented progression model:
$$\text{Concept} \rightarrow \text{Demonstration} \rightarrow \text{Guided Practice} \rightarrow \text{Independent Execution}$$

- **Format:** Weekly masterclasses combined with rigorous, independent lab execution.
- **Evaluation:** Weekly deliverables, hands-on exploitation proofs, and industry-standard technical reporting.

---

## 🗓️ 12-Week Curriculum Roadmap

| Month | Phase / Focus Area | Weeks | Core Objectives |
| :---: | :--- | :---: | :--- |
| **Month 1** | **Reconnaissance, Scanning & Web Basics** | W01 - W04 | OSINT, Nmap Mastery, Vulnerability Mapping, OWASP Top 10 |
| **Month 2** | **Internal Network & Active Directory** | W05 - W08 | Privilege Escalation, Pivoting, Kerberoasting, Domain Dominance |
| **Month 3** | **Advanced Operations & Capstone** | W09 - W12 | Evasion, C2 Deployment, Cloud Hacking, End-to-End Simulation |

---

## 🔴 Detailed Weekly Task Breakdown

<details>
<summary><b>📂 Click to expand Month 1: Reconnaissance, Scanning & Web Basics (Weeks 01 - 04)</b></summary>

### Week 01: Advanced Reconnaissance & Attack Surface Mapping
- **Objective:** Master information gathering and digital footprinting without detection.
- **Tasks & Execution:**
  - **Task 01:** Passive OSINT & Subdomain Enumeration (Subfinder, Assetfinder, Amass, CRT.sh, DNS Dumpster).
  - **Task 02:** Infrastructure & Technology Profiling (Wappalyzer, WhatWeb, Google Dorking for `.env` & `robots.txt`).
  - **Task 03:** GitHub Dorking & Credential Leaks (GitHacker, searching for hardcoded API keys & AWS secrets).
  - **Task 04:** Visual Reconnaissance (Httpx live asset verification, Aquatone/Gowitness screenshot generation).
- **Weekly Deliverable:** *The Reconnaissance Report* (Executive Summary, Clean CSV Asset List, Tech Map).

### Week 02: Network Enumeration & Service Vulnerability Discovery
- **Objective:** Transition from broad recon to targeted network scanning and service fingerprinting.
- **Tasks & Execution:**
  - **Task 01:** Advanced Nmap Scanning (TCP Connect `-sT`, SYN Stealth `-sS`, UDP `-sU`, Timing Templates `-T4`).
  - **Task 02:** Service Fingerprinting & Banner Grabbing (Version detection `-sV`, Netcat/Telnet banners, Enum4linux).
  - **Task 03:** Nmap Scripting Engine - NSE (Discovery/Safe scripts, Vuln scripts `--script vuln`, CVE mapping).
  - **Task 04:** Stealth & Firewall Evasion (Packet fragmentation `-f`, Decoys `-D`, Source Port Spoofing).
- **Weekly Deliverable:** *The Scanning & Enumeration Report* (Nmap output logs, Service Table, Evasion Results).

### Week 03: Vulnerability Assessment & Initial Exploitation
- **Objective:** Map discovered services to known CVEs and gain an initial foothold.
- **Tasks & Execution:**
  - **Task 01:** Web Directory & Parameter Discovery (ffuf, Dirsearch, Gobuster with SecLists, Arjun parameter discovery).
  - **Task 02:** CVE Mapping & Exploit Research (Searchsploit CLI, NVD/Exploit-DB lookup, RCE validation).
  - **Task 03:** CMS Vulnerability Scanning (WPScan plugins & username enumeration, JoomScan).
  - **Task 04:** The First Shell (`msfconsole`, payload configuration `LHOST`/`RHOST`, manual Netcat reverse shells).
- **Weekly Deliverable:** *The Vulnerability & Foothold Report* (Vulnerability Matrix, Web Discovery logs, PoC screenshots).

### Week 04: Web Application Penetration Testing (OWASP Top 10)
- **Objective:** Identify and exploit web-based vulnerabilities using standard methodologies.
- **Tasks & Execution:**
  - **Task 01:** Burp Suite Mastery (FoxyProxy setup, Proxy interception, Repeater replay, Intruder brute-forcing).
  - **Task 02:** Injection Attacks (Manual SQLi extraction, SQLMap automation, OS command injection).
  - **Task 03 & 04:** Broken Access Control (IDOR, parameter tampering) & XSS/File Inclusion (`/etc/passwd` LFI).
- **Weekly Deliverable:** *The OWASP Top 10 Audit Report* (Steps to Reproduce, Impact Analysis, Remediation Advice).

</details>

<details>
<summary><b>📂 Click to expand Month 2: Internal Network & Privilege Escalation (Weeks 05 - 08)</b></summary>

### Week 05: Post-Exploitation & Privilege Escalation
- **Objective:** Elevate privileges from a low-level shell to Root/SYSTEM and establish persistence.
- **Tasks & Execution:**
  - **Task 01:** Linux Privilege Escalation (Sudo misconfigs, SUID permissions, LinPEAS, Dirty Pipe exploit).
  - **Task 02:** Windows Privilege Escalation (WinPEAS, PowerUp, unquoted service paths, PrintSpoofer).
  - **Task 03 & 04:** Establishing Persistence (Cron jobs, Windows Scheduled Tasks) & Data Exfiltration.
- **Weekly Deliverable:** *The Post-Exploitation Report* (Escalation steps, tool breakdown, persistence verification).

### Week 06: Lateral Movement & Network Pivoting
- **Objective:** Reach isolated internal hosts through compromised gateway nodes.
- **Tasks & Execution:**
  - **Task 01 & 02:** Internal Network Discovery & Pivoting (SSH dynamic port forwarding `-D`, Chisel, Proxychains).
  - **Task 03:** Credential Dumping & Harvesting (Mimikatz LSASS dump, `/etc/shadow`, Hashcat cracking).
  - **Task 04:** Lateral Movement Techniques (Pass-the-Hash `psexec.py`, Evil-WinRM).
- **Weekly Deliverable:** *The Lateral Movement Report* (Network Diagram, tunneling commands, credential evidence).

### Week 07: Active Directory Enumeration & Kerberos Attacks
- **Objective:** Map Windows Domain architecture and exploit Kerberos authentication weaknesses.
- **Tasks & Execution:**
  - **Task 01 & 02:** Understanding AD Architecture & Quiet Enumeration (PowerView, BloodHound/SharpHound).
  - **Task 03:** AS-REP Roasting (`DONT_REQ_PREAUTH` users, Impacket-GetNPUsers, Hashcat).
  - **Task 04:** Kerberoasting (Requesting SPN tickets via Rubeus, cracking ticket hashes).
- **Weekly Deliverable:** *The AD Enumeration & Kerberos Report* (AD Map, BloodHound Shortest Path graphs, hardening advice).

### Week 08: AD Domain Dominance & Advanced Persistence
- **Objective:** Achieve total Domain Administration and enterprise forest control.
- **Tasks & Execution:**
  - **Task 01:** LLMNR/NBT-NS Poisoning (Responder listener, NTLMv2 hash harvesting).
  - **Task 02 & 03:** Weak ACLs/GPO Abuse & Golden/Silver Ticket Attacks (DCSync hash extraction).
  - **Task 04:** DCSync & NTDS.dit Extraction (`secretsdump.py`, full database dump).
- **Weekly Deliverable:** *The Domain Dominance Report* (Attack chain flow, ticket artifact breakdown, multi-tier hardening).

</details>

<details>
<summary><b>📂 Click to expand Month 3: Advanced Operations & Capstone (Weeks 09 - 12)</b></summary>

### Week 09: AV/EDR Evasion & Defensive Bypassing
- **Objective:** Bypass Windows Defender, AMSI, and EDR controls.
- **Tasks & Execution:**
  - **Task 01 & 02:** Payload Obfuscation (`shikata_ga_nai`) & Bypassing AMSI (memory patching).
  - **Task 03 & 04:** LOLBAS Binaries (Certutil, Regsvr32) & Process Injection/Hollowing in C++/C#.
- **Weekly Deliverable:** *The Evasion & Stealth Report* (Detection comparison table, AMSI bypass steps).

### Week 10: C2 Frameworks & Phishing Infrastructure
- **Objective:** Deploy professional C2 infrastructure and launch simulated phishing campaigns.
- **Tasks & Execution:**
  - **Task 01 & 02:** C2 Framework Deployment (Sliver/Havoc setup) & Weaponizing Documents (Macro documents, HTML smuggling).
  - **Task 03 & 04:** Phishing Infrastructure (GoPhish setup, login page cloning) & Domain Spoofing (SPF, DKIM, DMARC).
- **Weekly Deliverable:** *The Initial Access & C2 Report* (C2 dashboard view, GoPhish campaign analytics).

### Week 11: Cloud Security & Modern Infrastructure
- **Objective:** Exploit cloud misconfigurations (AWS/Azure) and container environments.
- **Tasks & Execution:**
  - **Task 01 & 02:** Cloud Recon (S3Scanner, CloudEnum) & Exploiting SSRF for Metadata (`169.254.169.254`).
  - **Task 03 & 04:** Attacking IAM & Azure (Pacu framework) & Container/Kubernetes Security (Docker socket escapes).
- **Weekly Deliverable:** *The Cloud & Infrastructure Audit Report* (Cloud asset map, metadata exploitation log).

### Week 12: The Capstone Project (Full Attack Chain Simulation)
- **Objective:** Execute an end-to-end simulated cyber attack from external recon to Domain Dominance.
- **Tasks & Execution:**
  - **Task 01 & 02:** Scoping & Rules of Engagement (ROE) + Full Cyber Kill Chain Execution.
  - **Task 03 & 04:** Post-Engagement Cleanup & The Boardroom Final Report Presentation.
- **Weekly Deliverable:** *The Cyberster Graduation Report* (Comprehensive 30+ page professional penetration testing report).

</details>

---

## 🛠️ Essential Toolkit Mastered
- **Recon & OSINT:** Amass, Subfinder, Assetfinder, WhatWeb, Wappalyzer, GitHacker.
- **Scanning & Enumeration:** Nmap, Netcat, Enum4linux, ffuf, Dirsearch, WPScan.
- **Exploitation & Web:** Metasploit, Burp Suite, SQLMap, Searchsploit, Impacket.
- **Post-Exploitation & AD:** LinPEAS, WinPEAS, Mimikatz, BloodHound, Rubeus, Responder, PowerView.
- **C2 & Evasion:** Sliver, Havoc, GoPhish, Custom Obfuscators, LOLBAS binaries.

---

<div align="center">

### 📊 Repository Statistics
![GitHub Streak](https://github-readme-streak-stats.herokuapp.com?user=DaniyalShahid&theme=tokyonight&hide_border=true)

*Maintained with 💻 and ☕ by **Daniyal Shahid** • CYBERSTER Batch 2*

</div>
