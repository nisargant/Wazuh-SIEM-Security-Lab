# Wazuh SIEM Security Lab

![Platform](https://img.shields.io/badge/Platform-Ubuntu%20%7C%20Windows-blue)
![SIEM](https://img.shields.io/badge/SIEM-Wazuh-green)
![Monitoring](https://img.shields.io/badge/Monitoring-Sysmon-orange)
![License](https://img.shields.io/badge/License-MIT-yellow)

A hands-on **Security Information and Event Management (SIEM)** lab built using **Wazuh**, **Sysmon**, **Ubuntu Server**, and **Windows 11** to demonstrate centralized log collection, endpoint monitoring, threat detection, and vulnerability assessment.

![Dashboard](Screenshots/09-agent-security-overview-dashboard.png)

---

## Table of Contents

- Quick Summary
- Setup
- Project Overview
- Lab Architecture
- Technologies Used
- Features
- Project Screenshots
- Verification Commands
- Skills Demonstrated
- Learning Outcomes
- Repository Structure
- Future Improvements

---

## Quick Summary

- **SIEM Platform:** Wazuh
- **Endpoint OS:** Windows 11
- **Server OS:** Ubuntu Server
- **Log Collection:** Wazuh Agent
- **Event Monitoring:** Sysmon
- **Vulnerability Detection:** Enabled

---

## Setup

1. Install Ubuntu Server.
2. Install Wazuh Manager.
3. Install Wazuh Indexer.
4. Install Wazuh Dashboard.
5. Install the Wazuh Agent on Windows 11.
6. Install and configure Sysmon.
7. Verify communication between the Windows endpoint and the Wazuh server.
8. Monitor security events and perform vulnerability assessment using the Wazuh Dashboard.

---

## Project Overview

This project demonstrates the deployment and configuration of a **Wazuh SIEM** environment capable of:

- Collecting Windows endpoint logs
- Monitoring system activity using Sysmon
- Detecting security events
- Performing vulnerability assessment
- Centralizing logs through the Wazuh Dashboard

---

## Lab Architecture

```text
Windows 11 Endpoint
       │
       │ Sysmon Logs
       ▼
Wazuh Agent
       │
       ▼
Wazuh Manager
       │
       ▼
Wazuh Indexer
       │
       ▼
Wazuh Dashboard
```

---

## Technologies Used

- Wazuh
- Sysmon
- Windows 11
- Ubuntu Server
- Linux
- PowerShell

---

## Features

- SIEM Deployment
- Windows Endpoint Monitoring
- Sysmon Integration
- Centralized Log Collection
- Threat Detection
- Vulnerability Assessment
- Security Dashboard
- Agent Monitoring

---

# Project Screenshots

## 1. Wazuh Dashboard (Before Agent Registration)

![Dashboard](Screenshots/01-wazuh-dashboard-home-before-agent.png)

---

## 2. Wazuh Manager Service Running

![Manager](Screenshots/02-wazuh-manager-service-running.png)

---

## 3. Wazuh Indexer Service Running

![Indexer](Screenshots/03-wazuh-indexer-service-running.png)

---

## 4. Wazuh Dashboard Service Running

![Dashboard Service](Screenshots/04-wazuh-dashboard-service-running.png)

---

## 5. Active Wazuh Agent

![Active Agent](Screenshots/05-wazuh-active-agents-dashboard.png)

---

## 6. Sysmon Installed

![Sysmon](Screenshots/06-sysmon-service-installed.png)

---

## 7. Sysmon Event Logs

![Logs](Screenshots/07-sysmon-event-logs-generated.png)

---

## 8. Wazuh Agent Service Running

![Agent](Screenshots/08-wazuh-agent-service-running.png)

---

## 9. Agent Security Overview

![Overview](Screenshots/09-agent-security-overview-dashboard.png)

---

## 10. Vulnerability Detection Overview

![Vulnerability](Screenshots/10-vulnerability-detection-overview.png)

---

## 11. High Severity Vulnerabilities

![High](Screenshots/11-high-severity-vulnerabilities.png)

---

## 12. Medium Severity Vulnerabilities

![Medium](Screenshots/12-medium-severity-vulnerabilities.png)

---

## 13. Low Severity Vulnerabilities

![Low](Screenshots/13-low-severity-vulnerabilities.png)

---

## Verification Commands

See the complete setup and verification guide in **[Commands.md](Commands.md)**.

---

## Skills Demonstrated

- SIEM Deployment
- Linux Administration
- Windows Event Logging
- Endpoint Security
- Threat Detection
- Vulnerability Management
- PowerShell
- Ubuntu Server
- Log Analysis
- Security Monitoring

---

## Learning Outcomes

Through this project, I gained practical experience in:

- Deploying and configuring a Wazuh SIEM environment
- Managing Wazuh Manager, Indexer, and Dashboard services
- Integrating Windows endpoints using the Wazuh Agent
- Configuring Sysmon for advanced Windows event logging
- Monitoring endpoint activity through a centralized dashboard
- Performing vulnerability detection and analysis
- Troubleshooting Linux services and agent communication

---

## Repository Structure

```text
Wazuh-SIEM-Security-Lab
│
├── README.md
├── Commands.md
├── LICENSE
└── Screenshots
    ├── 01-wazuh-dashboard-home-before-agent.png
    ├── 02-wazuh-manager-service-running.png
    ├── 03-wazuh-indexer-service-running.png
    ├── 04-wazuh-dashboard-service-running.png
    ├── 05-wazuh-active-agents-dashboard.png
    ├── 06-sysmon-service-installed.png
    ├── 07-sysmon-event-logs-generated.png
    ├── 08-wazuh-agent-service-running.png
    ├── 09-agent-security-overview-dashboard.png
    ├── 10-vulnerability-detection-overview.png
    ├── 11-high-severity-vulnerabilities.png
    ├── 12-medium-severity-vulnerabilities.png
    └── 13-low-severity-vulnerabilities.png
```

---

## Future Improvements

- Configure Active Response
- Enable Email Alerting
- Integrate MITRE ATT&CK Mapping
- Develop Custom Detection Rules
- Monitor Multiple Windows Endpoints
- Integrate Threat Intelligence Feeds

---

# 👨‍💻 Author

**Nisarga N T**

Aspiring SOC Analyst | SIEM | Threat Detection | Incident Response

**GitHub:** https://github.com/nisargant

**LinkedIn:** https://linkedin.com/in/nisarga-n-t

This project was created for educational purposes to demonstrate SIEM deployment, endpoint monitoring, vulnerability assessment, and security event analysis using Wazuh.

---

# 📄 License

This project is licensed under the MIT License.
