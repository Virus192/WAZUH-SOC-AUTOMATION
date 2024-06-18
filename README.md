# WAZUH SOC PROJECT
 # Security Operations Automation with Wazuh, Shuffle and TheHive 

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
 <div>
    <img src="https://imgur.com/a/M582nJf" />
</div>
 
 
## Project Overview

### Steps and Procedure

1. **🔰 Setup Wazuh Manager:**
- Install and configure a Wazuh Manager on a Ubuntu Server to centrally manage security monitoring.
2. **🔰 Deploy Wazuh Agents and Sysmon:**
- Install Wazuh agents on Windows 10 machines to collect security logs.
- Deploy Sysmon to enhance Windows event logging with detailed system activity.
3. **🔰 Configure Log Forwarding:**
- Configure Wazuh agents and Sysmon to forward security logs to the Wazuh Manager server for centralized monitoring.
4. **🔰 Prepare Credential Dumping Attack:**
- Use PowerShell scripts to simulate a credential dumping attack on the Windows 10 machine.
- Execute the attack to retrieve credentials and escalate privileges.
5. **🔰 Monitor Logs with Wazuh:**
- Monitor security logs on the Wazuh Manager server for alerts related to the credential dumping attack.
6. **🔰 Integrate Shuffle SOAR:**
- Integrate Wazuh Manager with the Shuffle SOAR platform for automated incident response.
7. **🔰 Automated Incident Handling:**
- Configure Shuffle SOAR to receive alerts from Wazuh and trigger automated response actions.
- Define workflows to analyze, contain, and mitigate security incidents automatically.
8. **🔰 Incident Management with TheHive:**
- Integrate Shuffle SOAR with TheHive case management platform for centralized incident handling.
- Create cases in TheHive for detected security incidents and assign them to SOC analysts for further investigation.
9.**🔰 Alert Notification via Email:**
- Configure Shuffle SOAR to send email notifications to SOC analysts for immediate response and analysis of critical security alerts.
10. **🔰 Documentation and Reporting:**
- Document the project steps, configurations, and integration details for future reference.
- Generate reports summarizing the project outcomes, including detected security incidents and response effectiveness.

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

- 🔰 Improved Efficiency: SOAR tools automate repetitive tasks such as alert triaging, enrichment, and response actions, reducing the time and effort required by security analysts. This allows analysts to focus on more critical tasks that require human decision-making.

- 🔰 Faster Response Times: Automation in SOAR tools accelerates incident response by executing predefined workflows and response actions in real-time or near real-time. This speed is crucial in mitigating threats before they escalate.

- 🔰 Consistency in Response: SOAR tools ensure consistent response actions across incidents by following predefined playbooks or workflows. This consistency helps maintain security best practices and reduces the likelihood of human error.

- 🔰 Enhanced Collaboration: SOAR platforms facilitate collaboration among different teams within the organization, such as security operations, IT, and incident response teams. This collaboration is essential for effective incident management and resolution.

- 🔰 Integration Capabilities: SOAR tools integrate with various security technologies, including SIEMs, threat intelligence platforms, endpoint detection and response (EDR) solutions, and ticketing systems. This integration allows for seamless data sharing and orchestration of security tools.

- 🔰 Scalability: As organizations grow and face increasing volumes of security alerts and incidents, SOAR tools can scale to handle higher workloads without a proportional increase in manpower.

- 🔰 Centralized Visibility and Reporting: SOAR platforms provide centralized visibility into security incidents, automation workflows, and response metrics. This visibility enables security teams to monitor performance, track metrics, and generate reports for compliance and improvement purposes.

- 🔰 Cost Efficiency: By automating routine tasks and optimizing resource allocation, SOAR tools help organizations achieve cost efficiencies in their security operations.

Overall, SOAR tools play a crucial role in modern cybersecurity operations by combining orchestration, automation, and response capabilities to improve security posture, reduce response times, and enhance operational efficiency.

---

For detailed step-by-step instructions, configurations, and integration details, please refer to the project report document included in this repository.

