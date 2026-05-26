<div align="center">

# Small Home SOC Lab: SIEM + Jira Integration & Elastic

### Security Operations Center (SOC) Workflow using Elastic SIEM & Jira

<img src="https://img.shields.io/badge/SIEM-Elastic-blue?style=for-the-badge&logo=elastic" />
<img src="https://img.shields.io/badge/Ticketing-Jira-blue?style=for-the-badge&logo=jira" />
<img src="https://img.shields.io/badge/Cybersecurity-SOC-red?style=for-the-badge" />
<img src="https://img.shields.io/badge/Status-Active-success?style=for-the-badge" />

</div>

---

## Overview

This project demonstrates how to build a **Home Security Operations Center (SOC) Lab** by integrating **Elastic SIEM** with **Jira** for incident tracking and resolution.

The lab simulates real-world workflows where detected security events are logged in **Elastic Security** and automatically pushed into **Jira** for structured monitoring, escalation, and remediation.

---

# Objectives

<ul>
<li>Deploy Elastic SIEM to detect and manage incidents</li>
<li>Integrate Jira for ticketing and workflow management</li>
<li>Showcase the incident lifecycle: Detection → Tracking → Resolution</li>
<li>Build a reproducible SOC learning environment</li>
</ul>

---

# Architecture

<div align="center">

```text
┌──────────────────────┐
│  Security Events     │
│ (Logs / Alerts)      │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│    Elastic SIEM      │
│ Detection & Cases    │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│        Jira          │
│ Ticket Management    │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│ Incident Resolution  │
│ & Feedback Workflow  │
└──────────────────────┘
```

</div>

---

# Components

## 🔹 Elastic SIEM

- Detects and logs security incidents  
- Monitors operational anomalies  
- Provides dashboards for case management  
- Tracks alerts and incident timelines  

### Example Events
- Platform slowness  
- Failed transactions  
- Authentication failures  
- Suspicious activities  

---

## 🔹 Jira via atlassian

- Receives incidents as tickets Image link: https://github.com/wouafotalla/soc-alert-siem-jira/blob/main/Screenshot%202026-05-25%209.46.14%20PM.png
- Tracks issue ownership and priorities, Image link: https://github.com/wouafotalla/soc-alert-siem-jira/blob/main/Screenshot%202026-05-25%209.49.35%20PM.png
- Monitors ticket lifecycle and resolution  
- Supports SOC investigation workflows  

---

## Integration Flow

<div align="center">

```text
Elastic Alert
      ↓
Elastic Case Created
      ↓
Jira Ticket Generated
      ↓
SOC Investigation
      ↓
Issue Resolution
      ↓
Case Closure & Feedback
```

</div>

---



# Features

Elastic SIEM Monitoring  
Incident Case Management  
Jira Ticket Automation  
Security Alert Workflow  
SOC Dashboard Visualization  
Incident Lifecycle Tracking  

## 1️Procedure
```bash
git[https://github.com/wouafotalla/soc-alert-siem-jira/edit/main/README] Steps
```

---

## 2️Deploy Elastic Stack

Install:
- Elasticsearch
- Elastic Security

## 3️Configure Jira Integration

- Create Jira API token and copy it
- 1) https://support.atlassian.com/atlassian-account/docs/manage-api-tokens-for-your-atlassian-account/
  2) https://github.com/wouafotalla/soc-alert-siem-jira/blob/main/Screenshot%202026-05-26%202.08.01%20AM.png
  3) https://github.com/wouafotalla/soc-alert-siem-jira/blob/main/Screenshot%202026-05-26%202.10.44%20AM.png
- Configure webhooks/API integration  
- Connect Elastic Cases to Jira  

---

## 4️Generate Test Alerts

Simulate:
- Failed logins  
- Platform outages  
- Suspicious activity  

---

## 5️Monitor the Incident Workflow

Observe:
- Elastic alerts  
- Jira ticket creation  
- Investigation workflow  
- Resolution lifecycle   

# Future Improvements I will do

- Add automated response actions  
- Integrate Slack notifications  
- Add phishing detection rules  
- Simulate brute-force attacks  
- Integrate Wazuh or Suricata  

---

<div align="center">

</div>
