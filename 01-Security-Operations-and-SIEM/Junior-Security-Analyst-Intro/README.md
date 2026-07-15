# Lab: Junior Security Analyst Intro

**Role:** Junior Security Analyst

## 🎯 Objective
To understand the core responsibilities of a Junior Security Analyst, explore the Security Operations Center (SOC) structure, and execute a standard incident handling workflow to mitigate a simulated cyber threat.

## 🚀 Execution Steps
1. **Monitoring & Alert Detection:** 
   * Monitored the SIEM (Security Information and Event Management) dashboard to review incoming security events. 
   * Identified a "Critical" level alert indicating a successful SSH login from a suspicious, unauthorized IP address.
2. **Investigation & Threat Enrichment:** 
   * Utilized Open-Source Intelligence (OSINT) tools, such as AbuseIPDB, Cisco Talos, and IP Hunter, to investigate the source IP.
   * Discovered that the IP originated from China and was flagged for historical malicious activities, including Port Scanning, operating as a Command and Control (C2) Server, and distributing the PlugX malware.
3. **Escalation & Remediation:** 
   * Declared an official security Incident due to the confirmation of a successful system compromise by a known malicious actor. 
   * Escalated the case to the Senior Analyst and SOC Manager for deeper forensic analysis.
   * Remediated the immediate threat by actively blocking the malicious IP on the Firewall and adding an incident comment to halt potential damage.

## 📊 Results & Evidence
* Successfully triaged a critical SSH login alert, verified the malicious nature of the IP using threat intelligence, and mitigated the immediate risk by enforcing a firewall block rule.

> 📸 SIEM DashBoard<img width="614" height="566" alt="image" src="https://github.com/user-attachments/assets/f2370755-ecbd-41c2-b903-3484bd709952" />
> 📸 Siem DashBoard<br><img width="578" height="239" alt="image" src="https://github.com/user-attachments/assets/0e3d548e-f3cd-4a8f-b261-2e57e3d565a5" />

> 📸 Check IP Address<img width="583" height="533" alt="image" src="https://github.com/user-attachments/assets/8ab712e9-80b0-47e9-8582-8fbfe9295f0c" />

> 📸 Escalate Ticket<img width="586" height="535" alt="image" src="https://github.com/user-attachments/assets/f22244ed-42ec-4961-91ff-969c37d5d148" />

> 📸 Blocking IP Address<img width="621" height="523" alt="image" src="https://github.com/user-attachments/assets/cad88381-b02c-453d-94be-bbd424fe4940" />


## 🧠 Key Takeaways
* **SOC Team Structure:** Gained a clear understanding of the SOC hierarchy, recognizing that Junior Analysts perform the initial triage, while Senior Analysts, Engineers, Managers, and Incident Responders handle complex analysis, system maintenance, and severe enterprise breaches.
* **SIEM as a Central Hub:** Learned that SIEM platforms are the primary operational tool for SOC teams, providing continuous monitoring, log aggregation, and real-time threat detection.
* **The Incident Handling Workflow:** Realized that practical cybersecurity defense requires a systematic approach: Monitoring the environment, Investigating alerts with external intelligence, Escalating confirmed threats, and applying immediate Remediation to protect the organization.
