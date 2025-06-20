# TryHackMe Room: Defensive Security Intro - Notes

## 🛡️ What is Defensive Security?

Defensive Security is the practice of protecting systems, networks, and data from unauthorized access, attacks, or damage. Unlike Offensive Security, which seeks vulnerabilities to exploit them, Defensive Security focuses on:

* **Preventing** intrusions from happening
* **Detecting** intrusions when they happen and responding to them effectively

Blue Teams handle Defensive Security tasks.

---

## 🔐 Core Areas of Defensive Security

### 1. **User Cyber Security Awareness**

* Teaching users how to avoid phishing, social engineering, and malware attacks

### 2. **Asset Management**

* Keeping a list of all hardware and software to know what needs protection

### 3. **Patching Systems**

* Updating software and systems to fix vulnerabilities (weaknesses)

### 4. **Preventative Security Devices**

* **Firewalls**: Control incoming and outgoing network traffic
* **IPS (Intrusion Prevention Systems)**: Block malicious activity based on rules/signatures

### 5. **Logging and Monitoring**

* Detect and alert suspicious behavior or unauthorized devices

---

## 🏢 Security Operations Center (SOC)

A team responsible for monitoring systems, detecting threats, and responding to cyber incidents.

**Main SOC tasks:**

* Detecting **vulnerabilities**, **policy violations**, **unauthorized access**, and **network intrusions**
* Working with Threat Intelligence to understand and anticipate attacks

### 📡 Threat Intelligence

* Collects, analyzes, and uses information about threats and attackers
* Helps organizations prepare for and respond to cyber threats

**Sources:**

* Internal (e.g. system/network logs)
* External (e.g. forums, open-source intelligence)

Goal: Create a **threat-informed defense** strategy.

---

## 🔍 DFIR - Digital Forensics and Incident Response

### 📁 Digital Forensics

Investigating digital devices to find evidence of a cybercrime or intrusion.

**Focus areas:**

* **File System**: Analyze deleted files, created files, and activity logs
* **System Memory**: Capture RAM to detect malware running in memory
* **System Logs**: Events recorded by the OS, even after attacker tries to hide their traces
* **Network Logs**: Monitor data packets (traffic) to see what entered/left the network

### 🚨 Incident Response

Steps taken after detecting a cyber incident:

1. **Preparation**
2. **Detection & Analysis**
3. **Containment, Eradication & Recovery**
4. **Post-Incident Activity (lessons learned/report)**

---

## 💀 Malware Analysis

Analyzing malicious software to understand its behavior and damage.

**Types of Malware:**

* **Virus**: Infects other programs and spreads
* **Trojan**: Looks harmless, hides a malicious function
* **Ransomware**: Encrypts files and demands payment

**Analysis Types:**

* **Static Analysis**: Study code without running it (requires assembly knowledge)
* **Dynamic Analysis**: Run malware in a sandbox to see what it does


## 🖥️ SIEM - Security Information and Event Management

A tool used in SOC to:

* Collect data from multiple sources (logs, systems, devices)
* Display alerts and incidents in one dashboard

**Example alerts:**

* Failed login attempts
* Connections from unknown IP addresses

SOC analysts review these alerts and identify real threats.


## 🧠 Key Terms:

* **Red Team**: Offensive Security (attackers)
* **Blue Team**: Defensive Security (defenders)
* **SOC**: Monitors and defends systems
* **DFIR**: Responds to incidents and investigates them
* **Malware**: Malicious software
* **SIEM**: Aggregates logs and raises alerts
* **Threat Intelligence**: Info about enemies to plan better defense
* **Network Packet**: Small chunk of data sent over a network
* **Data Breach**: When sensitive data is stolen or leaked
* **Flag**: A hidden string used to prove task completion (e.g. THM{...})
