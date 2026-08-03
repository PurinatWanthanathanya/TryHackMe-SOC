# Lab: Introduction to SOAR

**Role:** Junior Security Analyst / SOC Analyst Trainee

## 🎯 Objective
To understand the architectural components and capabilities of Security Orchestration, Automation, and Response (SOAR), evaluate how automated Playbooks streamline repetitive SOC workflows, and apply the "Human-in-the-Loop" model to balance automated containment with analyst decision-making.

## 🚀 Execution Steps
1. **SOAR Core Capabilities & Tool Orchestration:** 
   * Analyzed how SOAR platforms address critical SOC challenges—such as alert fatigue and disconnected tooling—through three core pillars: **Orchestration** (integrating disparate security tools via APIs), **Automation** (executing repetitive scripts), and **Response** (triggering containment actions).
2. **Playbook Execution & Workflow Analysis:** 
   * Evaluated standard **SOAR Playbooks** designed to automatically ingest raw alerts, extract Indicators of Compromise (IOCs), and enrich data using external Threat Intelligence feeds without manual analyst intervention.
   * Investigated automated response actions, such as isolating compromised endpoints or blocking malicious IP addresses on perimeter firewalls.
3. **Human-in-the-Loop Decision Governance:** 
   * Differentiated between tasks suitable for full automation (data collection, IOC enrichment, initial triage) and those requiring **Human-in-the-Loop** validation.
   * Implemented checkpoint approvals within automated workflows, ensuring high-risk containment actions or ambiguous alerts are validated by a SOC analyst before final execution.

## 📊 Results & Evidence
* Successfully mapped SOAR orchestration workflows, analyzed automated Playbook execution for alert enrichment, and demonstrated governance by applying human-led approval checkpoints on high-risk response actions.

> 📸 Phishing Playbook<br><img width="1434" height="1140" alt="image" src="https://github.com/user-attachments/assets/de16b56f-f3fb-40ae-a5f6-984578004f87" />

> 📸 CVE Patching Playbook<br><img width="3000" height="962" alt="image" src="https://github.com/user-attachments/assets/7995694b-3cce-4ee4-865e-8d71a7ae3ea9" />

> 📸 Case Ticket<br><img width="527" height="331" alt="image" src="https://github.com/user-attachments/assets/e10857cf-3cba-4497-8c48-2960a37d97c0" />

> 📸 Threat Intel<br><img width="522" height="264" alt="image" src="https://github.com/user-attachments/assets/4c36a55c-7bf3-4ae0-acf6-ea7d2bfb8833" />

> 📸 Data Extraction<br><img width="514" height="266" alt="image" src="https://github.com/user-attachments/assets/47f11997-6076-4dad-bc01-9b32d2e3a669" />

> 📸 Reputation Checks<br><img width="521" height="257" alt="image" src="https://github.com/user-attachments/assets/95e31612-54b9-48dd-8eeb-757091efffe1" />

> 📸 Course of Action<br><img width="523" height="329" alt="image" src="https://github.com/user-attachments/assets/17a854a6-cac1-46d5-a25b-4bd967ba237d" />

## 🧠 Key Takeaways
* **Automate Labor, Preserve Judgment:** Learned the core philosophy of modern security operations—SOAR automates the repetitive "labor" (collecting logs, querying threat feeds, and writing initial tickets), liberating SOC analysts to focus their "judgment" on critical analysis and strategic response.
* **Orchestration vs. Automation:**
  * **Automation** is doing a single repetitive task programmatically (e.g., a script checking an IP against VirusTotal).
  * **Orchestration** is connecting multiple tools together to execute an entire operational workflow (e.g., SIEM triggers an alert $\rightarrow$ SOAR enriches IOCs via Threat Intel $\rightarrow$ Ticket is created $\rightarrow$ EDR isolates the machine).
* **The Necessity of "Human-in-the-Loop":** Recognized that while SOAR can execute containment at machine speed, critical actions (such as disabling an executive's account or shutting down a production server) must require human validation to prevent business-disrupting false positives.
