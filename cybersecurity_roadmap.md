# Cybersecurity Roadmap
## System Requirements & Lab Setup
Minimum for smooth practice (affordable student setup):
CPU: Intel i5 / Ryzen 5 (quad-core)
RAM: 8GB (can run basic VMs, but 16GB is highly recommended for smoother labs)
Storage: 256GB SSD (faster than HDD; 512GB better for multiple VMs)
OS: Windows 10/11 or Linux (Ubuntu) as host
Virtualization support enabled in BIOS (Intel VT-x / AMD-V)

Recommended software:
VirtualBox (free) or VMware Workstation Player (free for non-commercial use)
Kali Linux VM (offensive practice)
Ubuntu / Windows Server VMs (targets for attacks & blue team analysis)
Wireshark, Burp Suite (Community), VS Code, Python
VPN account for TryHackMe / HackTheBox connectivity

Optional but useful:
External HDD/SSD (for VM storage)
Cloud credits (AWS / GCP student credits for cloud security practice)

## Phase 0 : Quick orientation (1 week)
Goal: understand the big picture (what cybersec is, blue vs red, simple career map).
Watch: a short “intro to cybersecurity” lecture (picoCTF’s intro lecture series is beginner-friendly). ()
Read: TryHackMe’s “Introduction to Cyber Security” module to see sample labs (gives both offensive & defensive views). ()
## Phase 1 : Very Basic / Foundations (4–6 weeks)
Goal: get comfortable with computers, Linux, basic networking and simple CTF puzzles.
What to learn (theory):
Basic OS concepts (what processes/files are), command line basics (ls, cd, cat, grep).
Networking fundamentals: IP, TCP/UDP, DNS, HTTP, common ports.
Basic scripting: Python (small scripts), Bash basics.


Hands-on (platforms & rooms):
TryHackMe: Pre-Security / Complete Beginner & Linux Fundamentals Part 1 — interactive browser labs that teach CLI and networking basics. Start here. ()
picoCTF: do starters from their “Get Started” page — excellent for absolute beginners and explains CTFs. ()
YouTube / Tutorials:
John Hammond — beginner videos and challenge walkthroughs (great mix of explanations + demos). ()
Weekly checklist:
Week 1: Finish TryHackMe “Introduction to Cyber Security”. ()
Week 2: Complete TryHackMe “Linux Fundamentals Part 1”. ()
Week 3: Solve 5 picoCTF beginner problems. ()
Week 4: Build 3 tiny Python scripts (port scanner, simple file parser).
Lab setup:
Install Kali Linux VM.
Set up a small network: one Kali VM (attacker) + one Ubuntu VM (victim).
Practice ping, netcat, nmap on your own LAN/VMs.
Projects:
Simple Port Scanner in Python.
Create a cheat sheet of 50 Linux commands with examples.
Build a mini password strength checker in Python.
Write a report on OWASP Top 10 with examples from websites you use.
## Phase 2 : Beginner → Lower-Intermediate (8–10 weeks)
Goal: practice basic pentesting, web vulnerabilities, enumeration, tooling.
What to learn:
Web fundamentals + OWASP Top 10 concepts (SQLi, XSS, LFI/RFI).
Recon & scanning (nmap, dirb/gobuster).
Basics of exploitation workflow (enumerate → exploit → escalate).
Hands-on (platforms & rooms/machines):
TryHackMe learning paths: follow the Web & Offensive paths (crypto & web rooms, vuln labs). TryHackMe’s free guides list a progression from tooling → web → CTF practice. ()
Hack The Box: Starting Point — a linear, beginner intro to HTB and pentesting workflows. Great next step after TryHackMe. ()
Example HTB easy boxes to attempt (once on HTB): Legacy or Arctic (easy Windows boxes with SMB / ColdFusion themes) — good for practicing SMB and web exploitation. ()
YouTube / Walkthroughs:
IppSec — excellent HTB machine walkthroughs (deep step-by-step). Start watching IppSec playlists for HTB Starting Point. ()
John Hammond — walkthroughs and conceptual videos (Kali tooling, CTF techniques). ()
Weekly checklist:
Week 1–2: TryHackMe web rooms (e.g., basic web injection & evasion). ()
Week 3–4: Complete full HackTheBox Starting Point sequence & watch one IppSec walkthrough per machine. ()
Week 5–6: Solve 10 picoCTF medium problems (crypto, web, forensics). ()
Practice targets (repeat cycle):
Do 1 web room + 1 linux room + 1 HTB easy box per week.
Keep a learning diary: commands used, enumeration notes, privilege escalation steps.
Lab setup:
Expand VM lab: Windows 10 VM (trial), Ubuntu server (web app).
Install vulnerable apps: DVWA (Damn Vulnerable Web App), Juice Shop.
Projects:
Web App Pentest Report: Run SQLi/XSS on DVWA/Juice Shop and write a professional report.
Network Recon Project: Use Nmap + Gobuster to map services of your own VM network.
Log Analysis Mini Project: Collect syslogs and use a simple ELK stack / Splunk Free / Wazuh to visualize.
CTF Portfolio: Document picoCTF / TryHackMe challenges solved with writeups.




## Phase 3 : Intermediate (3–6 months)
Goal: automated tooling, exploitation patterns, Windows/AD, basic DFIR and blue-team concepts.
What to learn:
Privilege escalation on Linux & Windows, AD basics and Kerberos concepts.
Log analysis, SIEM basics, and incident response playbooks. ()
Reverse engineering & basic malware analysis foundations (optionally).
Hands-on (platforms & rooms/machines):
TryHackMe: “Active Directory” learning path and Blue Team paths — many AD/Windows labs (privilege escalation, bloodhound concepts). ()
Hack The Box: move to Easy→Medium machines (do writeups after solving). Use HTB Academy and Starting Point guidance if stuck. ()
picoCTF / CTFs: tackle harder categories (reverse, pwn basics) to expand skill set. ()
YouTube / Playlists (study + follow along):
IppSec — medium and advanced HTB walkthroughs. ()
John Hammond — malware, blue team and advanced CTF walkthroughs. ()
Weekly checklist:
1 AD/Windows lab + 1 medium HTB machine + 1 blue team lab per week.
Start contributing to writeups or make your own notes — this cements learning.
Lab setup:
Build a small Active Directory lab (Windows Server + Windows 10 client).
Install security tools: BloodHound, Mimikatz (in lab only).
Install SIEM (Wazuh or Splunk Free) on a VM.
Projects:
Active Directory Attack & Defense Project: Attack AD with Kerberoasting & defend with logs.
SOC Mini Simulator: Forward logs (Windows Event, Sysmon, Suricata) into Wazuh/Splunk, create detection rules.
Incident Report Simulation: Pick a malware traffic sample (from), analyze PCAP, and write a report.
Threat Intel Dashboard: Use APIs (VirusTotal, AbuseIPDB) with Python to flag malicious IPs.
## Phase 4 : Advanced & Specialization (ongoing)
Goal: pick a track (Red, Blue, DFIR, AppSec, Cloud) and gain domain depth.
Specialization suggestions & resources:
Red Team / Offensive: HTB Pro Labs, Realistic networks, exploit dev, buffer overflows — follow IppSec and John Hammond for techniques. ()
Blue Team / DFIR: Incident response playbooks, malware traffic analysis, SIEM rules, threat intel feeds (VirusTotal, Talos). ()
OSINT: resources like LeakPeek, Intelligence X, HaveIBeenPwned. ()
Cloud Security: Google Cloud Skills Boost labs and cloud CTFs. ()
Advanced tracks tasks:
Build a home lab (VMs / AD domain / simulated company).
Regularly solve HTB medium+ boxes and try red-team emulations.
Start writing blog posts, GitHub repos and public writeups; teach others.
Lab setup:
Create a multi-VM network simulating a small company (AD, web server, mail server, SIEM).
Set up cloud labs using free credits (AWS/GCP).
Projects:
Red Team Project: Do a full penetration test on your lab, document findings as if for a client.
Blue Team Project: Create custom SIEM detection rules for MITRE ATT&CK techniques.
Malware Analysis Project: Reverse engineer a sample with x64dbg or strings/PEStudio.
OSINT Project: Use OSINT tools (HaveIBeenPwned, IntelX, LeakPeek) to research a fake target and produce a threat intel report.
Capstone Project: Combine red + blue → Attack your lab, collect logs, then produce a forensic & detection report.
## Recommended canonical resources (short list)
TryHackMe paths — Pre-Security / Complete Beginner / Web / Linux fundamentals. ()
Hack The Box — Starting Point and curated easy boxes (Legacy, Arctic etc.). ()
picoCTF — beginner→intermediate CTF problems and tutorials. ()
YouTube channels: IppSec (HTB walkthroughs), John Hammond (CTF & tutorials). ()

## Daily / weekly practice routine (practical)
Daily (30–60 min): one TryHackMe room or picoCTF problem. ()
Weekly (3–6 hours): 1 HTB Starting Point / easy box + watch a walkthrough after trying on your own. ()
Monthly: write a public writeup for one machine/room you solved.
## How to use walkthroughs without spoiling learning
Try to solve for 1–3 hours on your own.
If stuck, watch a walkthrough but pause frequently and replicate steps. IppSec and John Hammond are ideal for this method. ()
## Quick starter checklist you can follow
Create accounts: TryHackMe, HackTheBox, picoCTF. ()
Do TryHackMe Introduction to Cyber Security + Linux Fundamentals Part 1. ()
Solve 3 picoCTF beginner problems. ()
Start HTB Starting Point after finishing TryHackMe basics. ()
Subscribe to IppSec & John Hammond; watch 1 walkthrough per week. ()
## For More Resources you can go to











# Free Courses for Each Phase
## Free / Entry-Free Certifications / Training & Certs
## Common Paid or Widely Recognized Certifications
These are general certifications (some expensive), often seen as career-milestones. Suitable for later phases or as goals once skills and experience are built.









## Suggested Certification Roadmap by Phase
Here’s a suggested timeline: which certifications or training you might aim for in each phase of your learning journey.










# Websites

