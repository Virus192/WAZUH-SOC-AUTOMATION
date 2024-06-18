# WAZUH SOC
 # Security Operations Automation with Wazuh and Shuffle

## Strengthening Defenses and Automating Incident Detection and Response

### Presented by: Abdulazeez Mohammed

## Introduction

In response to the evolving cybersecurity landscape, this project aims to fortify organizational defenses against emerging threats. Key components include:

- Implementing a Wazuh Manager on Ubuntu Server for streamlined security monitoring.
- Deploying Wazuh Agents and Sysmon on Windows 10 for efficient log collection.
- Configuring log forwarding and conducting simulated attacks for monitoring.
- Integrating Shuffle SOAR and TheHive for automated incident response and centralized management.

## Tools Required

- **Windows 10 Pro**
  - RAM: 4GB
  - Cores: 2
  - Storage: 50GB
- **Wazuh**
  - RAM: 8GB+
  - SSD: 50GB+
  - OS: Ubuntu Server 22.04 LTS
- **TheHive**
  - RAM: 8GB+
  - SSD: 50GB+
  - OS: Ubuntu Server 22.04 LTS
- **Sysmon64.exe**
- **Shuffle**
- **Wazuh Agent**

## Objectives and Logical Diagram

The project comprised several key phases to address specific aspects of the organization's Security Operation needs.

## Project Overview

### Steps and Procedure

1. **Install and Configure Target-PC (Windows 10 Pro) on Oracle VirtualBox**
2. **Configure Sysmon and Wazuh Agent** to forward security logs to the Wazuh Manager server.
3. **Install and Configure a Wazuh Manager** on Ubuntu Server using DigitalOcean.
4. **Install Wazuh Agents on Windows 10** to collect security logs.
5. **Prepare Credential Dumping Attack** using PowerShell scripts.
6. **Monitor Security Logs** on the Wazuh Manager server for alerts.
7. **Install and Configure TheHive** on Ubuntu Server for case management.
8. **Configure Shuffle SOAR** to receive alerts from Wazuh and trigger automated response actions.
9. **Integrate Shuffle SOAR with TheHive** for centralized incident handling.
10. **Configure Shuffle SOAR to Send Email Notifications** to SOC analysts.
11. **Document Project Steps, Configurations, and Integration Details** for future reference.
12. **Generate Reports Summarizing Project Outcomes**.

## Detailed Installation and Configuration Steps

### Install and Configure Target-PC (Windows 10 Pro) on Oracle VirtualBox

- Download Windows 10 ISO from [Microsoft](https://www.microsoft.com/en-us/software-download/windows10).
- Create a new virtual machine in VirtualBox and allocate appropriate resources.
- Mount the Windows 10 ISO and install the OS.

### Configure Sysmon and Wazuh Agent

- Extract and run Sysmon with the sysmonconfig.xml file.
- Install the Wazuh Manager to obtain the API key for integrating the Wazuh agent.

### Install and Configure Wazuh Manager on Ubuntu Server

- Create a DigitalOcean account and set up a droplet with Ubuntu Server 22.04.
- Install Wazuh using the provided script and configure it for centralized monitoring.

### Prepare Credential Dumping Attack

- Download Mimikatz and run a simulated credential dumping attack.
- Monitor logs and create rules in Wazuh for detecting Mimikatz activity.

### Configure TheHive and Shuffle SOAR

- Install prerequisites for TheHive, including Java, Cassandra, and ElasticSearch.
- Configure TheHive for case management and integrate it with Shuffle SOAR.
- Create and automate workflows in Shuffle SOAR for incident response.

## Conclusion

This project successfully implemented advanced security measures and demonstrated the importance of SOAR tools for incident detection and response in a SOC environment.

## Recommendations

- Continuous Improvement
- Training and Skill Development
- Collaboration and Communication
- Integration and Automation
- Regular Evaluation and Review

## Importance of Using SOAR Tools

- Rapid Incident Response
- Enhanced Efficiency
- Improved Threat Detection

---

For detailed step-by-step instructions, configurations, and integration details, please refer to the project report document included in this repository.

