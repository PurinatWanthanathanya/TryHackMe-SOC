# Lab: Introduction to SIEM

**Role:** Junior Security Analyst

## 🎯 Objective
To understand the core architecture and features of a Security Information and Event Management (SIEM) system, including log aggregation, normalization, and how detection rules are utilized to monitor both host-centric and network-centric environments.

## 🧠 Key Concepts & Takeaways

### 1. The Necessity of SIEM
*   **Centralized Log Collection:** Without a SIEM, logs are scattered across different endpoints, servers, and firewalls. Investigating an incident by logging into machines individually (e.g., via SSH or RDP) is inefficient. SIEM centralizes this via agents or APIs.
*   **Normalization & Correlation:** Different machines output logs in different formats. SIEM normalizes these logs into a standard format (Parsing) and correlates them (e.g., suspicious VPN login + file share access + PowerShell execution) to detect complex attack patterns.
*   **Real-time Alerting & Dashboards:** SIEM platforms run continuous detection rules against ingested logs to trigger alerts and present visual insights via dashboards.

### 2. Host-Centric vs. Network-Centric Logs
*   **Host-Centric:** Logs generated directly on the device (Windows, Linux, Servers), recording internal activities such as user logins, process executions, Registry modifications, and PowerShell commands. 
    * *Example:* Windows Event Viewer (using Event IDs) or Linux `/var/log` directories (`auth.log`, `cron`, etc.).
*   **Network-Centric:** Logs generated when devices communicate over the network or access the internet. Captured by appliances like Firewalls, IDS/IPS, and Routers.
    * *Example:* SSH connections, FTP file transfers, web traffic, and VPN accesses.

### 3. Detection Rules & Logic
Detection rules act as logical expressions based on adversary behaviors. Examples include:
*   Triggering an alert for "Multiple Failed Login Attempts" (e.g., 5 failures in 10 seconds).
*   Triggering an alert when `WinEventLog` with Event ID `104` (Log clear) is detected, indicating an attacker covering their tracks.
*   Triggering an alert when Event ID `4688` (Process execution) runs a `whoami` command, which is a common post-exploitation technique.

## 🚀 Hands-On Analysis (Simulated SIEM Dashboard)

### 1. Alert Triage
*   Reviewed the SIEM dashboard and noticed a triggered alert regarding a suspicious process execution.
> 📸 Suspicious process execution Alerted<img width="550" height="499" alt="image" src="https://github.com/user-attachments/assets/80ab419d-b136-4aa3-b360-fa196d7af964" />

### 2. Investigation & Log Correlation
*   Drilled down into the specific event log to gather context.
*   Identified that a malicious cryptocurrency mining process named `cudominer.exe` was executed.
*   Traced the execution back to a specific user account (`Chris`) operating on the hostname `HR_02`.
*   Determined that the log source originated from a Windows endpoint.
> 📸 <img width="555" height="398" alt="image" src="https://github.com/user-attachments/assets/6bb1a6d3-1afd-49ca-81b0-9ea9cadf5ab1" />

### 3. Conclusion & Remediation
*   Analyzed the behavior and verified that it matched a crypto-mining infection. 
*   Declared the alert as a **True Positive**.
*   Took immediate remediation action by isolating the infected host (`HR_02`) from the network to prevent further spread, pending deeper forensic analysis.
> 📸 Analyze and choose verdict <img width="560" height="265" alt="image" src="https://github.com/user-attachments/assets/ed103c70-4ef5-422c-bd03-dcfe5131929b" />

## 💡 Note for Future Improvement
*   **Tuning False Positives:** I learned that if an alert turns out to be a False Positive, the correct procedure is to tune the detection rules. This reduces alert fatigue and prevents the SIEM from constantly triggering alerts on normal, legitimate business activities.
