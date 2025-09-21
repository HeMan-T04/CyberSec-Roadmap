# Cybersecurity Roadmap
## System Requirements & Lab Setup
Minimum for smooth practice (affordable student setup):
- CPU: Intel i5 / Ryzen 5 (quad-core)
- RAM: 8GB (can run basic VMs, but 16GB is highly recommended for smoother labs)
- Storage: 256GB SSD (faster than HDD; 512GB better for multiple VMs)
- OS: Windows 10/11 or Linux (Ubuntu) as host
- Virtualization support enabled in BIOS (Intel VT-x / AMD-V)

Recommended software:
- VirtualBox (free) or VMware Workstation Player (free for non-commercial use)
- Kali Linux VM (offensive practice)
- Ubuntu / Windows Server VMs (targets for attacks & blue team analysis)
- Wireshark, Burp Suite (Community), VS Code, Python
- VPN account for TryHackMe / HackTheBox connectivity

Optional but useful:
- External HDD/SSD (for VM storage)
- Cloud credits (AWS / GCP student credits for cloud security practice)

## Phase 0 : Quick orientation (1 week)
Goal: understand the big picture (what cybersec is, blue vs red, simple career map).
- Watch: a short “intro to cybersecurity” lecture (picoCTF’s intro lecture series is beginner-friendly). ([PicoCTF](https://picoctf.org/resources.html))
- Read: TryHackMe’s “Introduction to Cyber Security” module to see sample labs (gives both offensive & defensive views). ([TryHackMe](https://tryhackme.com/module/introduction-to-cyber-security))
## Phase 1 : Very Basic / Foundations (4–6 weeks)
Goal: get comfortable with computers, Linux, basic networking and simple CTF puzzles.

What to learn (theory):
- Basic OS concepts (what processes/files are), command line basics (ls, cd, cat, grep).
- Networking fundamentals: IP, TCP/UDP, DNS, HTTP, common ports.
- Basic scripting: Python (small scripts), Bash basics.


Hands-on (platforms & rooms):
- TryHackMe: Pre-Security / Complete Beginner & Linux Fundamentals Part 1 — interactive browser labs that teach CLI and networking basics. Start here. ([TryHackMe](https://tryhackme.com/path/outline/presecurity))
- picoCTF: do starters from their “Get Started” page — excellent for absolute beginners and explains CTFs. ([https://picoctf.org/get_started.html](https://picoctf.org/get_started.html))
YouTube / Tutorials:
- John Hammond — beginner videos and challenge walkthroughs (great mix of explanations + demos). ([https://www.youtube.com/@_JohnHammond](https://www.youtube.com/@_JohnHammond))

Weekly checklist:
- Week 1: Finish TryHackMe “Introduction to Cyber Security”. [TryHackMe](https://tryhackme.com/module/introduction-to-cyber-security)
- Week 2: Complete TryHackMe “Linux Fundamentals Part 1”. [TryHackMe](https://tryhackme.com/room/linuxfundamentalspart1)
- Week 3: Solve 5 picoCTF beginner problems. [picoCTF](https://picoctf.org/)
- Week 4: Build 3 tiny Python scripts (port scanner, simple file parser).

Lab setup:
- Install Kali Linux VM.
- Set up a small network: one Kali VM (attacker) + one Ubuntu VM (victim).
- Practice ping, netcat, nmap on your own LAN/VMs.

Projects:
- Simple Port Scanner in Python.
- Create a cheat sheet of 50 Linux commands with examples.
- Build a mini password strength checker in Python.
- Write a report on OWASP Top 10 with examples from websites you use.

## Phase 2 : Beginner → Lower-Intermediate (8–10 weeks)
Goal: practice basic pentesting, web vulnerabilities, enumeration, tooling.

What to learn:
- Web fundamentals + OWASP Top 10 concepts (SQLi, XSS, LFI/RFI).
- Recon & scanning (nmap, dirb/gobuster).
- Basics of exploitation workflow (enumerate → exploit → escalate).

Hands-on (platforms & rooms/machines):
- TryHackMe learning paths: follow the Web & Offensive paths (crypto & web rooms, vuln labs). TryHackMe’s free guides list a progression from tooling → web → CTF practice. [TryHackMe](https://tryhackme.com/resources/blog/free_path)
- Hack The Box: Starting Point — a linear, beginner intro to HTB and pentesting workflows. Great next step after TryHackMe. [Hack The Box Help Center](https://help.hackthebox.com/en/articles/6007919-introduction-to-starting-point)
- Example HTB easy boxes to attempt (once on HTB): Legacy or Arctic (easy Windows boxes with SMB / ColdFusion themes) — good for practicing SMB and web exploitation. [Hack The Box](https://www.hackthebox.com/machines/legacy)

YouTube / Walkthroughs:
- IppSec — excellent HTB machine walkthroughs (deep step-by-step). Start watching IppSec playlists for HTB Starting Point. [IppSec](https://www.youtube.com/channel/UCa6eh7gCkpPo5XXUDfygQQA)
- John Hammond — walkthroughs and conceptual videos (Kali tooling, CTF techniques). [John Hammond](https://www.youtube.com/%40_JohnHammond)

Weekly checklist:
- Week 1–2: TryHackMe web rooms (e.g., basic web injection & evasion). [TryHackMe](https://tryhackme.com/resources/blog/free_path)
- Week 3–4: Complete full HackTheBox Starting Point sequence & watch one IppSec walkthrough per machine. [Hack The Box Help Center](https://help.hackthebox.com/en/articles/6007919-introduction-to-starting-point)
- Week 5–6: Solve 10 picoCTF medium problems (crypto, web, forensics). [picoCTF](https://picoctf.org/)

Practice targets (repeat cycle):
- Do 1 web room + 1 linux room + 1 HTB easy box per week.
- Keep a learning diary: commands used, enumeration notes, privilege escalation steps.

Lab setup:
- Expand VM lab: Windows 10 VM (trial), Ubuntu server (web app).
- Install vulnerable apps: DVWA (Damn Vulnerable Web App), Juice Shop.

Projects:
- Web App Pentest Report: Run SQLi/XSS on DVWA/Juice Shop and write a professional report.
- Network Recon Project: Use Nmap + Gobuster to map services of your own VM network.
- Log Analysis Mini Project: Collect syslogs and use a simple ELK stack / Splunk Free / Wazuh to visualize.
- CTF Portfolio: Document picoCTF / TryHackMe challenges solved with writeups.

## Phase 3 : Intermediate (3–6 months)
Goal: automated tooling, exploitation patterns, Windows/AD, basic DFIR and blue-team concepts.

What to learn:
- Privilege escalation on Linux & Windows, AD basics and Kerberos concepts.
- Log analysis, SIEM basics, and incident response playbooks. [Hack The Box](https://www.hackthebox.com/blog/when-easy-isnt-easy)
- Reverse engineering & basic malware analysis foundations (optionally).

Hands-on (platforms & rooms/machines):
- TryHackMe: “Active Directory” learning path and Blue Team paths — many AD/Windows labs (privilege escalation, bloodhound concepts). [TryHackMe](https://tryhackme.com/path/outline/beginner)
- Hack The Box: move to Easy→Medium machines (do writeups after solving). Use HTB Academy and Starting Point guidance if stuck. [Hack The Box](https://www.hackthebox.com/blog/when-easy-isnt-easy)
- picoCTF / CTFs: tackle harder categories (reverse, pwn basics) to expand skill set. [picoCTF](https://picoctf.org/)

YouTube / Playlists (study + follow along):
- IppSec — medium and advanced HTB walkthroughs. [IppSec](https://www.youtube.com/channel/UCa6eh7gCkpPo5XXUDfygQQA)
- John Hammond — malware, blue team and advanced CTF walkthroughs. [John Hammond](https://www.youtube.com/%40_JohnHammond)

Weekly checklist:
- 1 AD/Windows lab + 1 medium HTB machine + 1 blue team lab per week.
- Start contributing to writeups or make your own notes — this cements learning.

Lab setup:
- Build a small Active Directory lab (Windows Server + Windows 10 client).
- Install security tools: BloodHound, Mimikatz (in lab only).
- Install SIEM (Wazuh or Splunk Free) on a VM.

Projects:
- Active Directory Attack & Defense Project: Attack AD with Kerberoasting & defend with logs.
- SOC Mini Simulator: Forward logs (Windows Event, Sysmon, Suricata) into Wazuh/Splunk, create detection rules.
- Incident Report Simulation: Pick a malware traffic sample (from [Malware Traffic Analysis](https://malware-traffic-analysis.net/)), analyze PCAP, and write a report.
- Threat Intel Dashboard: Use APIs (VirusTotal, AbuseIPDB) with Python to flag malicious IPs.

## Phase 4 : Advanced & Specialization (ongoing)
Goal: pick a track (Red, Blue, DFIR, AppSec, Cloud) and gain domain depth.

Specialization suggestions & resources:
- Red Team / Offensive: HTB Pro Labs, Realistic networks, exploit dev, buffer overflows — follow IppSec and John Hammond for techniques. [IppSec](https://www.youtube.com/channel/UCa6eh7gCkpPo5XXUDfygQQA)
- Blue Team / DFIR: Incident response playbooks, malware traffic analysis, SIEM rules, threat intel feeds (VirusTotal, Talos). [Medium](https://cyberkareem.medium.com/hackthebox-arctic-walkthrough-13e1920d0cca)
- OSINT: resources like LeakPeek, Intelligence X, HaveIBeenPwned. [TryHackMe](https://tryhackme.com/p/Learn.Linux)
- Cloud Security: Google Cloud Skills Boost labs and cloud CTFs. [TryHackMe](https://tryhackme.com/module/linux-fundamentals)

Advanced tracks tasks:
- Build a home lab (VMs / AD domain / simulated company).
- Regularly solve HTB medium+ boxes and try red-team emulations.
- Start writing blog posts, GitHub repos and public writeups; teach others.

Lab setup:
- Create a multi-VM network simulating a small company (AD, web server, mail server, SIEM).
- Set up cloud labs using free credits (AWS/GCP).

Projects:
- Red Team Project: Do a full penetration test on your lab, document findings as if for a client.
- Blue Team Project: Create custom SIEM detection rules for MITRE ATT&CK techniques.
- Malware Analysis Project: Reverse engineer a sample with x64dbg or strings/PEStudio.
- OSINT Project: Use OSINT tools (HaveIBeenPwned, IntelX, LeakPeek) to research a fake target and produce a threat intel report.
- Capstone Project: Combine red + blue → Attack your lab, collect logs, then produce a forensic & detection report.

## Recommended canonical resources (short list)
- TryHackMe paths — Pre-Security / Complete Beginner / Web / Linux fundamentals. [TryHackMe](https://tryhackme.com/path/outline/beginner)
- Hack The Box — Starting Point and curated easy boxes (Legacy, Arctic etc.). [Hack The Box Help Center](https://help.hackthebox.com/en/articles/6007919-introduction-to-starting-point)
- picoCTF — beginner→intermediate CTF problems and tutorials. [picoCTF](https://picoctf.org/)
- YouTube channels: IppSec (HTB walkthroughs), John Hammond (CTF & tutorials). [IppSec](https://www.youtube.com/channel/UCa6eh7gCkpPo5XXUDfygQQA) [John Hammond](https://www.youtube.com/%40_JohnHammond)

## Daily / weekly practice routine (practical)
- Daily (30–60 min): one TryHackMe room or picoCTF problem. [TryHackMe](https://tryhackme.com/room/linuxfundamentalspart1) [picoCTF](https://picoctf.org/)
- Weekly (3–6 hours): 1 HTB Starting Point / easy box + watch a walkthrough after trying on your own. [Hack The Box Help Center](https://help.hackthebox.com/en/articles/6007919-introduction-to-starting-point)
- Monthly: write a public writeup for one machine/room you solved.

## How to use walkthroughs without spoiling learning
- Try to solve for 1–3 hours on your own.
- If stuck, watch a walkthrough but pause frequently and replicate steps. IppSec and John Hammond are ideal for this method. [IppSec](https://www.youtube.com/channel/UCa6eh7gCkpPo5XXUDfygQQA) [John Hammond](https://www.youtube.com/%40_JohnHammond)
## Quick starter checklist you can follow
- Create accounts: TryHackMe, HackTheBox, picoCTF. [TryHackMe](https://tryhackme.com/) [Hack The Box](https://www.hackthebox.com/) [picoCTF](https://picoctf.org/)
- Do TryHackMe Introduction to Cyber Security + Linux Fundamentals Part 1. [TryHackMe](https://tryhackme.com/module/introduction-to-cyber-security)
- Solve 3 picoCTF beginner problems. [picoCTF](https://picoctf.org/)
- Start HTB Starting Point after finishing TryHackMe basics. [Hack The Box Help Center](https://help.hackthebox.com/en/articles/6007919-introduction-to-starting-point)
- Subscribe to IppSec & John Hammond; watch 1 walkthrough per week. [IppSec](https://www.youtube.com/channel/UCa6eh7gCkpPo5XXUDfygQQA) [John Hammond](https://www.youtube.com/%40_JohnHammond)

## For More Resources you can go to
[https://roadmap.sh/cyber-security](https://roadmap.sh/cyber-security)

# Free Courses for Each Phase

| Phase | Course | What It Covers / Why Good |
| --- | --- | --- |
| Phase 1 – Very Basic / Foundations | TryHackMe Cyber Security 101 path (free) [TryHackMe](https://tryhackme.com/path/outline/introtocyber) | Beginner friendly; introduces networking, cryptography, Linux, Windows basics, tools etc. Good starting point. () |
|  | SkillsBuild (Students) – Cybersecurity Fundamentals [SkillsBuild](https://skillsbuild.org/students/course-catalog/cybersecurity) | Covers basics: terminology, roles, encryption, attacker tactics. Great for understanding domain language. () |
|  | EC-Council Free Courses – “Free Cyber Security Courses & Certifications for Beginners” [EC-Council](https://www.eccouncil.org/cybersecurity-exchange/cyber-novice/free-cybersecurity-courses-beginners/) | Several foundational level courses (ethical hacking, network defense etc.). Good theory + some labs. () |
|  | Coursera “Cybersecurity for Everyone” (University of Maryland) (audit mode/free) [Coursera](https://www.coursera.org/courses?query=free&skills=Cybersecurity&utm_source=chatgpt.com) | Helps understand policy, risk, roles, infrastructure. Good for getting broad view. () |
| Phase 2 – Beginner → Intermediate | PortSwigger Web Security Academy (free) [PortSwigger](https://portswigger.net/web-security) | Web vulnerability labs & theory: SQLi, XSS, API, CSRF etc. Very hands-on. () |
|  | Microsoft Learn – Active Directory Domain Services learning path [Microsoft Learn](https://learn.microsoft.com/en-us/training/paths/active-directory-domain-services/) | For AD basics: domains, controllers, GPO, certificates etc. Helps setting up Windows environment, understanding directory services. () |
|  | ViaMonstra – “Mini-Course: Active Directory Security – Hardening Tips & Tricks” [ViaMonstra Online Academy](https://academy.viamonstra.com/courses/mini-course-active-directory-security-hardening-tips-and-tricks) | Short training (on-demand) focused on securing AD, good for learning defense & domain hardening. () |
| Phase 3 – Intermediate | Cybrary free content & labs [Cybrary](https://www.cybrary.it/free-content) | Has OSINT, intermediate courses, guided labs. Good for reconnaissance, deeper web, log analysis etc. () |
|  | ServerAcademy – Active Directory Fundamentals (free) [ServerAcademy](https://serveracademy.com/courses/active-directory-fundamentals/) | More in-depth AD work: creating/managing users, privileges, domain setup. Helps with Windows/AD labs. () |
|  | Fortinet Free Self-Paced Training for Cybersecurity Professionals [Fortinet](https://www.fortinet.com/training/cybersecurity-professionals) | Deeper defense-oriented courses: network security, cloud security, operations etc. Useful for blue-team labs. () |
| Phase 4 – Advanced & Specialization | Active Directory advanced / MCITP style AD courses from Cursa.app (“Free course Active Directory”) [Cursa](https://cursa.app/en/free-course/active-directory-heh) | More advanced AD config, policies, certificates, domain trust etc. Useful for Red/Blue specialization. () |
|  | EC-Council’s free Essential Series (if you qualify / for educators / students) for specialized tracks (Threat Intel, IoT security etc.) [EC-Council](https://www.eccouncil.org/cybersecurity-exchange/cyber-novice/free-cybersecurity-courses-beginners/) | Gives you access to specialized free modules for deeper knowledge. () |
|  | MyGreatLearning Free Cybersecurity Courses & Certificates (2025) [MyGreatLearning](https://www.mygreatlearning.com/cybersecurity/free-courses) | Helps explore topics like encryption, forensics etc., helpful for advanced project ideas. () |

# Free / Entry-Free Certifications / Training & Certs
| Certification / Certificate Program | What It Offers / Who Provides It | Phase(s) Suited |
| --- | --- | --- |
| ISC² Certified in Cybersecurity (CC) | Free self-paced training + exam (for a limited period via “One Million Certified” initiative). Entry-level, no prior experience needed. [ISC2](https://www.isc2.org/landing/1mcc) | Foundations / Phase 1 |
| EC-Council Essentials Series | Free foundational courses + certificate in topics like Ethical Hacking Essentials, Network Defense Essentials, Digital Forensics Essentials, SOC Essentials etc. [EC-Council](https://www.eccouncil.org/cybersecurity-exchange/cyber-novice/free-cybersecurity-courses-beginners/) | Foundations → Beginner / Phase 1-2 |
| Palo Alto Networks Cyberpedia Free Courses | Self-paced free courses in topics like “Introduction to Cybersecurity,” “Network Security,” “Fundamentals of SOC,” etc. (certificate of completion) [Palo Alto Networks](https://www.paloaltonetworks.com/cyberpedia/free-cybersecurity-education-courses) | Foundations / Phase 1 |
| Fortinet Free Self-Paced Training | No-cost curriculum including labs / free training around cloud security, zero-trust, operations etc. (not always full paid certs, but valuable credential/training with certificates) [Fortinet](https://www.fortinet.com/training/cybersecurity-professionals) | Phase 1 → Phase 2 |

# Common Paid or Widely Recognized Certifications
These are general certifications (some expensive), often seen as career-milestones. Suitable for later phases or as goals once skills and experience are built.
| Certification | Issuing Body | What It Covers / Requirements | Phase Suited / When to Target |
| --- | --- | --- | --- |
| Security+ | CompTIA | Broad covering of IT security fundamentals: identity, risk, threats, cryptography, etc. Good first official cert after basics. [Coursera](https://www.coursera.org/articles/popular-cybersecurity-certifications) | Phase 2 (Beginner → Intermediate) |
| Google Cybersecurity Certificate | Google / Coursera | Entry-level job-ready skills: Linux, networking, SIEM, incident response, etc. [Google](https://grow.google/certificates/cybersecurity/) | Phase 1 → Phase 2 |
| SSCP (Systems Security Certified Practitioner) | (ISC)² | More hands-on operational security skills (administration, monitoring, operations). Requires some experience. | Phase 2 → Phase 3 |
| CEH (Certified Ethical Hacker) | EC-Council | Ethical hacking methodologies, tools, offensive skills. Practical version is more advanced. | Phase 2 → Phase 3 (once decent hands-on) |
| OSCP (Offensive Security Certified Professional) | Offensive Security | Very hands-on penetration testing, lab-based exam; considered tough. | Phase 3 → Advanced |
| CISSP (Certified Information Systems Security Professional) | (ISC)² | Broad, senior level, covering many domains (governance, risk, operations, asset security etc.). Requires years of experience. [InfoSecurityEurope](https://www.infosecurityeurope.com/en-gb/blog/guides-checklists/top-10-cybsersecurity-certifications.html) | Phase 4 / Advanced |
| CISM (Certified Information Security Manager) | ISACA | Management + governance oriented; good for roles managing teams or policies. | Advanced / Phase 4 |
| CISA (Certified Information Systems Auditor) | ISACA | Audit, assurance, compliance of information systems; strong in governance, risk. | Advanced / Phase 4 |
| GIAC Certifications (GSEC, GCIH etc.) | GIAC (SANS) | Technical & specialized (for example incident handling, auditing, security essentials). Often hands-on. | Phase 3 → Advanced |


# Suggested Certification Roadmap by Phase
Here’s a suggested timeline: which certifications or training you might aim for in each phase of your learning journey.
| Phase | Recommended Free / Low-cost Certifications / Training | Goal Certs for that Phase |
| --- | --- | --- |
| Phase 1 (Foundations) | ISC² CC, EC-Council Essentials, Palo Alto free courses, Fortinet free courses | Google Cybersecurity Certificate, CompTIA Security+ |
| Phase 2 (Beginner → Intermediate) | Continue training, maybe do EC-Council / Fortinet more advanced modules; possibly apply for discount vouchers for Security+ or SSCP | CompTIA Security+, SSCP, CEH (if budget allows) |
| Phase 3 (Intermediate) | Labs + practice; possibly pay for full CEH or OSCP; take smaller certs in specialized domains (incident response, threat intel) | OSCP, specialized GIAC certs, more advanced EC-Council certs |
| Phase 4 (Advanced / Specialization) | Deep specialization; fewer free certs but earned experience; aim for senior certificates and maybe management ones | CISSP, CISM, CISA, specialized architect / management certs |


# Websites
Websites.xlsx provided in the repository 
[Websites.xlsx](./Websites.xlsx)
