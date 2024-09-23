# Dynamic Threat Detection Lab: Reverse Shells, Telemetry, and SIEM Analysis

## Overview
This project is part of a broader series focused on building a **SOC Automation Lab** that includes **Wazuh** for threat detection, **The Hive** for case management, and **Shuffle** for automating incident responses. The primary goal is to simulate a malware attack and analyze the resulting telemetry data using **Splunk** and **Sysmon**.

## Objective
This project simulates a real-world malware attack by utilizing **Nmap**, **msfvenom**, and **Metasploit**. The goal is to trigger telemetry data in **Sysmon**, analyze the data in **Splunk**, and automate the SOC operations using **Wazuh**, **The Hive**, and **Shuffle**.

## Skills Learned
- VM network configuration for secure malware testing.
- Using **Nmap** to identify vulnerabilities.
- Crafting and deploying malware using **msfvenom** and **Metasploit**.
- Analyzing telemetry data with **Sysmon** and **Splunk**.
- Automating SOC workflows with **Wazuh**, **The Hive**, and **Shuffle**.

## Tools Used
- **VirtualBox** & **VMware**
- **Kali Linux** (attacker)
- **Windows** (target)
- **Nmap**, **msfvenom**, **Metasploit**
- **Sysmon** for event monitoring
- **Splunk** for log analysis
- **Wazuh**, **The Hive**, **Shuffle** (SOC automation)

## Steps and Screenshots

### Step 1: VM Configuration for Safe Malware Testing
- Use **VirtualBox** with **Internal Network** for isolation and assign static IPs.

![Network Config](imgsrc)

### Step 2: Nmap Scan
- **Nmap** scan to identify open ports on the Windows target machine.

![Nmap Scan](imgsrc)

### Step 3: Creating Malware with msfvenom
- Generate reverse TCP shell payload disguised as resume.pdf.exe using **msfvenom**.

![msfvenom Payload](imgsrc)

### Step 4: Executing Reverse Shell
- **Metasploit** establishes a reverse shell between Kali and the Windows target.

![Reverse Shell](imgsrc)

### Step 5: Analyzing Telemetry in Splunk
- Use **Sysmon** and **Splunk** to detect malicious activity.

![Splunk Telemetry](imgsrc)

## Challenges and Solutions
- **Bypassing Antivirus**: Disable **Windows Defender** to execute the payload.
- **Telemetry Configuration**: Properly configure **Sysmon** and **Splunk** for comprehensive event tracking.

## Results
- Successfully simulated malware attack using **Metasploit**.
- Generated detailed telemetry for analysis.
- Developed detection rules to identify malicious behavior in **Splunk**.

## Learning Outcomes
- Mastered safe VM network configurations for malware testing.
- Gained practical experience with vulnerability scanning, malware creation, and telemetry analysis.
- Enhanced understanding of SOC operations using **Wazuh**, **The Hive**, and **Shuffle**.

## Next Steps
- Expand the SOC lab with additional endpoints.
- Automate incident response workflows using **Shuffle** and **Wazuh**.
