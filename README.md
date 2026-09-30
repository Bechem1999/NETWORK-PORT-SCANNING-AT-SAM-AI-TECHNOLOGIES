# 🛡️ NETWORK SCAN USING ZENMAP/Nmap

<div align="center">

[![Cybersecurity](https://img.shields.io/badge/Cybersecurity-Network_Security-red)](#)
[![Nmap](https://img.shields.io/badge/Nmap-Network_Scanning-4682B4)](https://nmap.org/)
[![Zenmap](https://img.shields.io/badge/Zenmap-Nmap_GUI-0066CC)](https://nmap.org/zenmap/)
[![Kali Linux](https://img.shields.io/badge/Kali_Linux-Security_Platform-557C94)](https://www.kali.org/)
[![Linux](https://img.shields.io/badge/Linux-Command_Line-FCC624)](#)
[![Networking](https://img.shields.io/badge/Networking-Network_Reconnaissance-green)](#)
[![Port Scanning](https://img.shields.io//badge/Port_Scanning-Network_Enumeration-blue)](#)
[![Service Detection](https://img.shields.io/badge/Service_Detection-Network_Analysis-purple)](#)
[![Ethical Hacking](https://img.shields.io/badge/Ethical_Hacking-Authorized_Testing-red)](#)
[![VirtualBox](https://img.shields.io/badge/VirtualBox-Lab_Environment-blue)](https://www.virtualbox.org/)
[![GitHub](https://img.shields.io/badge/GitHub-Project_Documentation-black)](#)

</div>

---

## 📌 Project Overview

This project demonstrates the practical use of **Zenmap**, the graphical interface associated with Nmap, for network reconnaissance and port scanning in a controlled cybersecurity laboratory environment.

The objective was to understand how network scanning can be used to identify reachable hosts, discover open ports, determine available services and collect information that can help build an initial picture of a target network.

The project was performed using **Kali Linux** within a controlled laboratory environment.

## 🧪 Lab Environment

**Operating System:** Kali Linux
**Assessment Type:** Network Reconnaissance / Port Scanning
**Primary Tool:** Zenmap / Nmap
**Lab Environment:** Virtualized security laboratory
**Purpose:** Educational cybersecurity and ethical hacking

---

## 🎯 Project Objectives

The main objectives of this project were to:

* Understand the purpose of network reconnaissance.
* Use Zenmap as a graphical interface for Nmap.
* Identify hosts available within an authorized laboratory network.
* Scan for open and closed ports.
* Identify services running on discovered ports.
* Interpret basic network-scanning results.
* Document scan findings using screenshots and saved outputs.
* Develop practical experience with network reconnaissance and enumeration.

---

## 🛠️ Tools & Technologies

| Tool / Technology | Purpose                                          |
| ----------------- | ------------------------------------------------ |
| `Zenmap`          | Graphical interface for Nmap network scanning    |
| `Nmap`            | Network discovery and port scanning              |
| `Kali Linux`      | Cybersecurity testing environment                |
| `VirtualBox`      | Virtualized laboratory environment               |
| `Linux Terminal`  | Command-line interaction and output management   |
| `GitHub`          | Project documentation and portfolio presentation |

---

## 🔍 What is Zenmap?

**Zenmap** provides a graphical interface for Nmap and makes it easier to configure scans, execute them and interpret the results.

Nmap is widely used for network discovery and security auditing. In a controlled laboratory, it can help identify:

* Hosts that respond to network probes
* Open ports
* Closed or filtered ports
* Running services
* Service versions where version detection is enabled
* Basic information about the target's network exposure

---

## 🔬 Methodology

The assessment followed a structured workflow:

```text
             AUTHORIZED TARGET
                    │
                    ▼
             TARGET IDENTIFICATION
                    │
                    ▼
              ZENMAP / NMAP
                    │
                    ▼
             HOST DISCOVERY
                    │
                    ▼
              PORT SCANNING
                    │
                    ▼
            SERVICE DETECTION
                    │
                    ▼
             RESULT ANALYSIS
                    │
                    ▼
          SCREENSHOTS & OUTPUTS
                    │
                    ▼
             FINAL DOCUMENTATION
```

The approach was designed to move from basic network discovery toward identification and interpretation of exposed services.

---

## 🖥️ Scanning Process

### 01 · Launching Zenmap

Zenmap was opened from the Kali Linux environment.

The target was entered into the appropriate target field, followed by selection of the required scan profile.

### 02 · Selecting the Scan

The scan configuration was selected according to the objective of the laboratory exercise.

The scan was then executed against the authorized target.

### 03 · Analysing the Results

After the scan completed, the results were reviewed to identify:

* Discovered hosts
* Open ports
* Port states
* Detected services
* Service information
* Other information returned by the scan

### 04 · Saving Evidence

The results were documented using screenshots and saved text outputs.

Example command-line output can also be saved using Linux redirection:

```bash
nmap <authorized-target> > scan_results.txt
```

To append additional results without overwriting the existing file:

```bash
nmap <authorized-target> >> scan_results.txt

## 📊 Findings

The following table can be updated with the actual results obtained during the laboratory scan.

| Port  | State    | Service      | 
| ---   | -------- | -------      |
|   135 | Open     | epmap        | 
|   139 | Open     | netbios-ssn  | 
|   445 | Open     | microsoft-ds | 


## 🧠 Key Skills Demonstrated

### 🔎 Network Reconnaissance

Understanding how information about a network can be collected before deeper security assessment.

### 🌐 Port Scanning

Identifying ports that are exposed or accessible on an authorized target.

### 🛠️ Service Enumeration

Interpreting information about services associated with discovered ports.

### 🐧 Linux

Working with Kali Linux and the command line.

### 📊 Result Analysis

Reading and interpreting scan results rather than simply running scanning tools.

### 📝 Technical Documentation

Recording commands, screenshots, outputs and findings in a reproducible format.

---

## ⚠️ Challenge Faced

One practical challenge encountered during the project was **saving the scan output in `.txt` format** for proper documentation.

Initially, the scan results were visible in the Kali Linux terminal, but I needed a reliable way to preserve the results as a text file so that they could be reviewed and included as project evidence.

### 💡 How I Resolved It

I used AI-assisted learning and troubleshooting to understand Linux output redirection and then tested the approach in the Kali Linux environment.

I learned that the `>` operator can redirect command output into a text file:

```bash
nmap <authorized-target> > scan_results.txt
```

I also learned that `>>` can be used to append additional results:

```bash
nmap <authorized-target> >> scan_results.txt
```

This solved the documentation problem and also improved my understanding of Linux command-line operations.

> **Key lesson:** AI was used as a learning and troubleshooting aid, while the commands were tested and verified in the laboratory environment.

---

## 📚 Lessons Learned

### 1. Network scanning requires a structured approach

A useful scan is not simply about running a command. The results need to be interpreted in relation to the target and assessment objective.

### 2. Open ports provide useful information

Open ports can indicate services that are accessible on a host and therefore deserve further investigation during an authorized assessment.

### 3. Service detection adds context

Knowing that a port is open is useful, but identifying the service associated with that port provides additional context.

### 4. Documentation is important

Saving screenshots and outputs makes the work reproducible and provides evidence of what was observed.

### 5. Troubleshooting is part of technical learning

The difficulty I experienced while saving outputs helped me develop a better understanding of Linux command-line redirection.

---

## 🛡️ Defensive Security Perspective

Network scanning can also be used from a defensive perspective.

Organizations can conduct authorized scans against their own infrastructure to determine:

* Which hosts are reachable.
* Which ports are exposed.
* Which services are accessible.
* Whether unnecessary services are running.
* Whether the external attack surface is larger than expected.

The information can then be used to reduce unnecessary exposure and improve network security.

---

## ⚖️ Ethical & Legal Disclaimer

This project is intended strictly for **educational purposes and authorized security testing**.

Do not use Zenmap, Nmap or any other scanning technique against systems or networks without explicit permission from the owner.

The techniques documented in this repository should be practiced only in controlled laboratories, training environments or authorized assessments.

---

# 👨‍💻 Author

ATEMLEFAC NKAFU BECHEM

Cybersecurity Engineer

# Cybersecurity #Python #Network port scanner #Cryptography #KaliLinux #EthicalHacking #CyberSecurityInternship #SAMAITechnologies
