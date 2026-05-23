# INTER VISION

## Network Reconnaissance and Footprinting 
![Platform](https://img.shields.io/badge/Platform-Kali_Linux-blue)
![Domain](https://img.shields.io/badge/Domain-Cybersecurity-red)
![Status](https://img.shields.io/badge/Status-Completed-success)

Network Reconnaissance and Footprinting is a cybersecurity minor project focused on ethical reconnaissance, footprinting, and network analysis using Kali Linux and open-source security tools. The project demonstrates how publicly accessible information about a target can be gathered and analyzed using standard reconnaissance methodologies.

---

# Project Overview

Reconnaissance and footprinting are the initial phases of cybersecurity assessment and ethical hacking. Attackers and security professionals use these techniques to gather information about domains, servers, services, DNS infrastructure, and exposed network resources.

This project demonstrates practical implementation of:

- WHOIS Enumeration
- DNS Enumeration
- MX and NS Record Analysis
- Subdomain Enumeration
- Google Dorking
- Ping Analysis
- Traceroute Analysis
- Web Server Fingerprinting
- Port Scanning using Nmap

The project was performed in a controlled and ethical environment using authorized public targets.

---

# Objectives

- Perform ethical reconnaissance on an authorized target
- Gather publicly available domain information
- Analyze DNS infrastructure
- Discover publicly accessible subdomains
- Perform network connectivity analysis
- Identify open ports and running services
- Understand the importance of footprinting in cybersecurity

---

# Tools and Technologies Used

| Tool       | Purpose                             |
| ---------- | ----------------------------------- |
| Kali Linux | Penetration Testing Environment     |
| Nmap       | Port Scanning and Service Detection |
| WHOIS      | Domain Information Gathering        |
| DIG        | DNS Enumeration                     |
| NSLOOKUP   | DNS Analysis                        |
| cURL       | HTTP Header Fingerprinting          |
| Sublist3r  | Subdomain Enumeration               |
| Ping       | Connectivity Analysis               |
| Traceroute | Network Path Analysis               |

---

# Project Structure

```text
INTER-VISION_Minor-Project/
│
├── README.md
├── .gitignore
│
├── docs/
│   ├── Minor_Project_Report.pdf
│   └── Minor_Project_Report.docx
│
├── diagrams/
│   ├── system_architecture.png
│   ├── network_topology.png
│   └── workflow_diagram.png
│
├── screenshots/
│   ├── whois.png
│   ├── dns_enum.png
│   ├── mx_lookup.png
│   ├── ns_lookup.png
│   ├── subdomain_enum.png
│   ├── google_dorking_1.png
│   ├── google_dorking_2.png
│   ├── google_dorking_3.png
│   ├── ping.png
│   ├── traceroute.png
│   ├── web_fingerprint.png
│   └── nmap_scan.png
│
├── cmds/
│   └── commands_used.txt
│
└── results/
    └── findings_summary.txt
```

---

# Reconnaissance Workflow

Target Selection  
↓  
WHOIS Enumeration  
↓  
DNS Enumeration  
↓  
Subdomain Discovery  
↓  
Google Dorking  
↓  
Network Analysis  
↓  
Web Fingerprinting  
↓  
Port Scanning  
↓  
Report Generation

---

# Commands Used

## WHOIS Enumeration

```bash
whois nmap.org
```

## DNS Enumeration

```bash
nslookup scanme.nmap.org
dig scanme.nmap.org
```

## MX Record Lookup

```bash
nslookup -type=mx nmap.org
dig mx nmap.org
```

## NS Record Lookup

```bash
nslookup -type=ns nmap.org
dig ns nmap.org
```

## Subdomain Enumeration

```bash
sublist3r -d nmap.org
```

## Network Connectivity Analysis

```bash
ping -c 4 scanme.nmap.org
```

## Traceroute Analysis

```bash
traceroute scanme.nmap.org
```

## Web Server Fingerprinting

```bash
curl -I http://scanme.nmap.org
```

## Port Scanning

```bash
nmap -F scanme.nmap.org
```

---

# Key Findings

- Public domain registration details were identified
- DNS infrastructure was successfully analyzed
- Multiple subdomains were discovered
- Publicly indexed web resources were identified
- Network latency and routing information were analyzed
- HTTP headers revealed web server information
- Open ports and active services were detected

---

# Screenshots Included

The repository contains categorized screenshots for:

- WHOIS Enumeration
- DNS Analysis
- MX and NS Record Enumeration
- Subdomain Enumeration
- Google Dorking
- Ping and Traceroute
- HTTP Fingerprinting
- Nmap Scanning

---

# Documentation

Complete project documentation is available in the `docs/` directory.

---

# Ethical Use Disclaimer

This project is developed strictly for educational and authorized cybersecurity assessment purposes only.

The techniques demonstrated in this repository must only be performed on systems and targets for which explicit permission has been obtained.

Unauthorized scanning, reconnaissance, or exploitation of systems is illegal and unethical.

---

# Future Enhancements

- Automated report generation
- Web-based dashboard integration
- Vulnerability assessment module
- AI-assisted reconnaissance analysis
- Scan history management

---

# Author

**M Rithwik Kumar**  
Cyber Security Engineering Student