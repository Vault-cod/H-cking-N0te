# Day 1 - Introduction to Cybersecurity
Date: April 18, 2026
Platform: TryHackMe
Path: Introduction to Cyber Security

---
## What I Learned Today

### 1. Offensive Security
Offensive security is about thinking like an attacker.
The goal is to find weaknesses in systems before 
real criminals do.

Key tool I used: Gobuster
Gobuster is a tool that brute-forces hidden pages 
on a website by trying hundreds of page names 
from a wordlist.

Command I ran: gobuster -u http://fakebank.thm -w wordlist.txt dir
- -u = the target website URL
- -w = the wordlist file to use
- dir = look for directories/pages

What happened:
Gobuster found a hidden page called /bank-transfer
(Status 200 = page exists and is accessible).
The page had no authentication so I was able to 
transfer money freely.

Vulnerability type: Broken Access Control
A page that should be private was left open 
with no login or verification required.

My first flag: BANK-HACKED ✅

---

### 2. Defensive Security
Defensive security is about protecting systems 
and responding to attacks.

Key areas covered:

SOC (Security Operations Center)
A team that monitors a company's network 24/7 
for malicious activity. They handle:
- Vulnerabilities
- Policy violations
- Unauthorized activity
- Network intrusions

Threat Intelligence
Gathering information about potential attackers —
who they are, how they attack, and why —
to prepare defenses in advance.

DFIR (Digital Forensics & Incident Response)
- Digital Forensics = investigating after an attack
  like a digital detective (file systems, logs,
  memory, network traffic)
- Incident Response = the plan to handle attacks

4 phases of Incident Response:
1. Preparation
2. Detection & Analysis
3. Containment, Eradication & Recovery
4. Post-Incident Review

Malware Analysis
Studying malicious software to understand 
how it works and how to stop it.

Types of malware:
- Virus — spreads and corrupts files
- Trojan Horse — looks legitimate but gives 
  attacker control
- Ransomware — encrypts files and demands payment

Two analysis methods:
- Static Analysis — studying code without running it
- Dynamic Analysis — running it in a safe environment
  and observing behavior

---

### 3. Careers in Cyber
Different roles in cybersecurity:

| Role | What they do |
|------|-------------|
| Security Analyst | Monitor & protect daily |
| Incident Responder | Handle active attacks |
| Digital Forensics | Investigate after attacks |
| Malware Analyst | Reverse engineer malware |
| Penetration Tester | Hack with permission |
| Red Teamer | Advanced simulated attacks |
| Security Engineer | Build security systems |

My target role: Penetration Tester → Red Teamer

Difference between Pentester and Red Teamer:
- Pentester finds vulnerabilities and reports them
- Red Teamer fully simulates a real criminal attack —
  breaking in, staying hidden for weeks, 
  avoiding all detection

How they get paid:
Most pentesters and red teamers work for 
cybersecurity consulting firms or go freelance.
They get hired per engagement, not permanently,
because companies only need testing occasionally.

---

## Key Terms Learned Today

| Term | Meaning |
|------|---------|
| Gobuster | Tool to find hidden web pages |
| Brute Force | Trying many options until one works |
| Status 200 | Page exists and loaded successfully |
| Broken Access Control | Page accessible without proper authorization |
| SOC | Team monitoring security 24/7 |
| Threat Intelligence | Info about potential attackers |
| DFIR | Digital Forensics & Incident Response |
| Malware | Malicious software |
| Virus | Malware that spreads between programs |
| Trojan Horse | Malware disguised as legitimate software |
| Ransomware | Malware that encrypts files for ransom |
| Pentester | Ethical hacker hired to find vulnerabilities |
| Red Teamer | Advanced attacker simulating real criminals |
| MTTD | Mean Time To Detect |
| MTTA | Mean Time To Acknowledge |
| MTTR | Mean Time To Recover |

---

## Rooms Completed
- [x] Offensive Security Intro
- [x] Defensive Security Intro
- [x] Careers in Cyber

---

## Reflection
Day 1 done. I learned the difference between 
offensive and defensive security, ran my first 
real hacking tool, found a hidden page on a 
fake bank, and transferred money as my first 
ever hack. I also learned all the major career 
paths in cybersecurity.

Target path: Jr Penetration Tester → Red Teamer

*The journey starts today.* 🔐
